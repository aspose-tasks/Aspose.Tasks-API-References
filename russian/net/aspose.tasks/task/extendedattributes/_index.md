---
title: "Task.ExtendedAttributes"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Task. Возвращает объект ExtendedAttributeCollection, содержащий значения расширенного атрибута"
type: docs
weight: 400
url: /ru/net/aspose.tasks/task/extendedattributes/
---
## Task.ExtendedAttributes property

Получает объект ExtendedAttributeCollection, содержащий значения расширенного атрибута.

```csharp
public ExtendedAttributeCollection ExtendedAttributes { get; }
```

## Примечания

Необходимо два элемента данных — указатель на таблицу расширенных атрибутов, который задаётся либо уникальным идентификатором, либо идентификатором поля, и значение, которое задаётся либо непосредственно значением, либо указателем на список значений.

## Примеры

Показывает, как читать расширенные атрибуты задачи.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// Создать определение расширенного атрибута
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Start, ExtendedAttributeTask.Start7, "Start 7");
project.ExtendedAttributes.Add(definition);

// Получить задачу с нулевым индексом
var tsk = project.RootTask.Children.GetById(1);

// Добавить расширенный атрибут
var extendedAttribute = definition.CreateExtendedAttribute();
extendedAttribute.DateValue = DateTime.Now;

// Также можно использовать следующий короткий синтаксис: ExtendedAttribute attribute = attributeDefinition.CreateExtendedAttribute(DateTime.Now);
tsk.ExtendedAttributes.Add(extendedAttribute);

// Создайте определение расширенного атрибута типа Text1
var taskExtendedAttributeText1Definition =
    ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text1, "Task City Name");

// Добавьте его в коллекцию расширенных атрибутов проекта
project.ExtendedAttributes.Add(taskExtendedAttributeText1Definition);

var newTask = project.RootTask.Children.Add("Task 1");

// Создайте расширенный атрибут из определения атрибута
var taskExtendedAttributeText1 = taskExtendedAttributeText1Definition.CreateExtendedAttribute();

// Назначьте значение сгенерированному расширенному атрибуту. Тип атрибута — "Text", следует использовать свойство "TextValue".
taskExtendedAttributeText1.TextValue = "London";

// Добавьте расширенный атрибут к задаче
newTask.ExtendedAttributes.Add(taskExtendedAttributeText1);

// Создайте определение расширенного атрибута типа Text2
var taskExtendedAttributeText2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text2,
    "Task Towns Name");

// Добавьте lookup‑значения для определения расширенного атрибута
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 1, StringValue = "Town1", Description = "This is Town1" });
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 2, StringValue = "Town2", Description = "This is Town2" });

// Добавьте его в коллекцию расширенных атрибутов проекта
project.ExtendedAttributes.Add(taskExtendedAttributeText2Definition);

var task2 = project.RootTask.Children.Add("Task 2");

// Создайте расширенный атрибут из определения поиска Text2 для Id 1
var taskExtendedAttributeText2 = taskExtendedAttributeText2Definition.CreateExtendedAttribute(taskExtendedAttributeText2Definition.ValueList[1]);

// Добавьте расширенный атрибут к задаче
task2.ExtendedAttributes.Add(taskExtendedAttributeText2);

// Создайте определение расширенного атрибута типа Duration2
var taskExtendedAttributeDuration2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Duration,
    ExtendedAttributeTask.Duration2,
    "Some duration");

// Добавьте значения поиска для определения расширенного атрибута
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 3, Duration = project.GetDuration(4, TimeUnitType.Hour), Description = "4 hours" });
taskExtendedAttributeDuration2Definition.AddLookupValue(new Value { Id = 4, Duration = project.GetDuration(1, TimeUnitType.Day), Description = "1 day" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 5, Duration = project.GetDuration(1, TimeUnitType.Hour), Description = "1 hour" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 6, Duration = project.GetDuration(10, TimeUnitType.Day), Description = "10 days" });

// Добавьте определение в коллекцию расширенных атрибутов проекта
project.ExtendedAttributes.Add(taskExtendedAttributeDuration2Definition);

var task3 = project.RootTask.Children.Add("Task 3");

// Создайте расширенный атрибут из определения поиска Duration2 для Id 3
var taskExtendedAttributeDuration2 =
    taskExtendedAttributeDuration2Definition.CreateExtendedAttribute(taskExtendedAttributeDuration2Definition.ValueList[3]);

// Добавьте расширенный атрибут к задаче
task3.ExtendedAttributes.Add(taskExtendedAttributeDuration2);

// Создайте определение расширенного атрибута типа Finish2
var taskExtendedAttributeFinish2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Finish,
    ExtendedAttributeTask.Finish2,
    "Some finish");

// Добавьте значения поиска для определения расширенного атрибута
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 7, DateTimeValue = new DateTime(1984, 01, 01, 00, 00, 01), Description = "This is Value2" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 8, DateTimeValue = new DateTime(1994, 01, 01, 00, 01, 01), Description = "This is Value3" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 9, DateTimeValue = new DateTime(2009, 12, 31, 00, 00, 00), Description = "This is Value4" });
taskExtendedAttributeFinish2Definition.AddLookupValue(new Value { Id = 10, DateTimeValue = DateTime.Now, Description = "This is Value6" });

// Добавьте определение в коллекцию расширенных атрибутов проекта
project.ExtendedAttributes.Add(taskExtendedAttributeFinish2Definition);

var task4 = project.RootTask.Children.Add("Task 4");

// Создайте расширенный атрибут из определения поиска Finish2 для Id 3
var taskExtendedAttributeFinish2 = taskExtendedAttributeFinish2Definition.CreateExtendedAttribute(taskExtendedAttributeFinish2Definition.ValueList[3]);

// Добавьте расширенный атрибут к задаче
task4.ExtendedAttributes.Add(taskExtendedAttributeFinish2);

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Чтение расширенных атрибутов для задач
foreach (var task in collector.Tasks)
{
    foreach (var attribute in task.ExtendedAttributes)
    {
        Console.WriteLine(attribute.FieldId);
        Console.WriteLine(attribute.ValueGuid);

        switch (attribute.AttributeDefinition.CfType)
        {
            case CustomFieldType.Date:
            case CustomFieldType.Start:
            case CustomFieldType.Finish:
                Console.WriteLine(attribute.DateValue);
                break;
            case CustomFieldType.Text:
                Console.WriteLine(attribute.TextValue);
                break;
            case CustomFieldType.Duration:
                Console.WriteLine(attribute.DurationValue.ToString());
                break;
            case CustomFieldType.Cost:
            case CustomFieldType.Number:
                Console.WriteLine(attribute.NumericValue);
                break;
            case CustomFieldType.Flag:
                Console.WriteLine(attribute.FlagValue);
                break;
            case CustomFieldType.Null:
            case CustomFieldType.RBS:
            case CustomFieldType.OutlineCode:
                return;
            default:
                return;
        }
    }
}

project.Save(OutDir + "ReadWriteTaskExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### См. также

* class [ExtendedAttributeCollection](../../extendedattributecollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


