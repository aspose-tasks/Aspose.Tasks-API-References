---
title: "ExtendedAttributeDefinition.CreateTaskDefinition"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "ExtendedAttributeDefinition метод. Фабричный метод, который создает простое определение расширенного атрибута, которое Microsoft Project отображает как None. Имеет CalculationType, равный None, и может использоваться только в задачах. Требуется указать customFieldType, fieldId и alias при вызове этого метода."
type: docs
weight: 40
url: /ru/net/aspose.tasks/extendedattributedefinition/createtaskdefinition/
---
## CreateTaskDefinition(CustomFieldType, ExtendedAttributeTask, string) {#createtaskdefinition}

Фабричный метод, который создает простое определение расширенного атрибута, которое Microsoft Project отображает как "None". Имеет [`CalculationType`](../calculationtype/) равный None и может использоваться только в задачах. Требуется указать *customFieldType*, *fieldId* и *alias* при вызове этого метода.

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeTask fieldId, string alias)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| customFieldType | CustomFieldType | Указанный тип [`CustomFieldType`](../../customfieldtype/). |
| fieldId | ExtendedAttributeTask | Указанный идентификатор поля [`ExtendedAttributeTask`](../../extendedattributetask/). |
| alias | Строка | Указанный строковый alias. |

### Возвращаемое значение

Создан экземпляр класса [`ExtendedAttributeDefinition`](../) с указанными *customFieldType*, *fieldId* и *alias*.

## Примеры

Используйте этот пример для создания пользовательского определения текстового поля:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

Показывает, как создать расширенные атрибуты задачи.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Создайте определение расширенного атрибута типа Text1
var taskExtendedAttributeText1Definition =
    ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text1, "Task City Name");

// Добавьте его в коллекцию расширенных атрибутов проекта
project.ExtendedAttributes.Add(taskExtendedAttributeText1Definition);

// Добавьте задачу в проект
var task = project.RootTask.Children.Add("Task 1");

// Создайте расширенный атрибут из определения атрибута
var taskExtendedAttributeText1 = taskExtendedAttributeText1Definition.CreateExtendedAttribute();

// Назначьте значение сгенерированному расширенному атрибуту. Тип атрибута — "Text", следует использовать свойство "TextValue".
taskExtendedAttributeText1.TextValue = "London";

// Добавьте расширенный атрибут к задаче
task.ExtendedAttributes.Add(taskExtendedAttributeText1);

project.Save(OutDir + "PlainTextExtendedAttribute_out.mpp", SaveFileFormat.Mpp);

var project4 = new Project(DataDir + "Blank2010.mpp");

// Создайте определение расширенного атрибута типа Text2
var taskExtendedAttributeText2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text2,
    "Task Towns Name");

// Добавьте lookup‑значения для определения расширенного атрибута
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 1, StringValue = "Town1", Description = "This is Town1" });
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 2, StringValue = "Town2", Description = "This is Town2" });

// Добавьте его в коллекцию расширенных атрибутов проекта
project4.ExtendedAttributes.Add(taskExtendedAttributeText2Definition);

// Добавьте задачу в проект
var task2 = project4.RootTask.Children.Add("Task 2");

// Создайте расширенный атрибут из определения поиска Text2 для Id 1
var taskExtendedAttributeText2 = taskExtendedAttributeText2Definition.CreateExtendedAttribute(taskExtendedAttributeText2Definition.ValueList[1]);

// Добавьте расширенный атрибут к задаче
task2.ExtendedAttributes.Add(taskExtendedAttributeText2);

project4.Save(OutDir + "TextExtendedAttributeWithLookup_out.mpp", SaveFileFormat.Mpp);

var project2 = new Project(DataDir + "Blank2010.mpp");

// Создайте определение расширенного атрибута типа Duration2
var taskExtendedAttributeDuration2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Duration,
    ExtendedAttributeTask.Duration2,
    "Some duration");

// Добавьте значения поиска для определения расширенного атрибута
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 2, Duration = project2.GetDuration(4, TimeUnitType.Hour), Description = "4 hours" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 3, Duration = project2.GetDuration(1, TimeUnitType.Day), Description = "1 day" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 4, Duration = project2.GetDuration(1, TimeUnitType.Hour), Description = "1 hour" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 7, Duration = project2.GetDuration(10, TimeUnitType.Day), Description = "10 days" });

// Добавьте определение в коллекцию расширенных атрибутов проекта
project2.ExtendedAttributes.Add(taskExtendedAttributeDuration2Definition);

// Добавьте задачу в проект
var task3 = project2.RootTask.Children.Add("Task 3");

// Создайте расширенный атрибут из определения поиска Duration2 для Id 3
var taskExtendedAttributeDuration2 =
    taskExtendedAttributeDuration2Definition.CreateExtendedAttribute(taskExtendedAttributeDuration2Definition.ValueList[3]);

// Добавьте расширенный атрибут к задаче
task3.ExtendedAttributes.Add(taskExtendedAttributeDuration2);

project2.Save(OutDir + "DurationExtendedAttributeWithLookup_out.mpp", SaveFileFormat.Mpp);

var project3 = new Project(DataDir + "Blank2010.mpp");

// Создайте определение расширенного атрибута типа Finish2
var taskExtendedAttributeFinish2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Finish,
    ExtendedAttributeTask.Finish2,
    "Some finish");

// Добавьте значения поиска для определения расширенного атрибута
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 2, DateTimeValue = new DateTime(1984, 01, 01, 00, 00, 01), Description = "This is Value2" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 3, DateTimeValue = new DateTime(1994, 01, 01, 00, 01, 01), Description = "This is Value3" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 4, DateTimeValue = new DateTime(2009, 12, 31, 00, 00, 00), Description = "This is Value4" });
taskExtendedAttributeFinish2Definition.AddLookupValue(new Value { Id = 7, DateTimeValue = DateTime.Now, Description = "This is Value6" });

// Добавьте определение в коллекцию расширенных атрибутов проекта
project3.ExtendedAttributes.Add(taskExtendedAttributeFinish2Definition);

// Добавьте задачу в проект
var task4 = project3.RootTask.Children.Add("Task 4");

// Создайте расширенный атрибут из определения поиска Finish2 для Id 3
var taskExtendedAttributeFinish2 = taskExtendedAttributeFinish2Definition.CreateExtendedAttribute(taskExtendedAttributeFinish2Definition.ValueList[3]);

// Добавьте расширенный атрибут к задаче
task4.ExtendedAttributes.Add(taskExtendedAttributeFinish2);

project3.Save(OutDir + "FinishExtendedAttributeWithLookup_out.mpp", SaveFileFormat.Mpp);
```

### См. также

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateTaskDefinition(ExtendedAttributeTask, string) {#createtaskdefinition_1}

Фабричный метод, который создает простое определение расширенного атрибута, отображаемое в Microsoft Project как "None". Он имеет [`CalculationType`](../calculationtype/) со значением None и может использоваться только в задачах. При вызове этого метода необходимо указывать *fieldId* и *alias*. Тип поля выводится из идентификатора поля.

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(ExtendedAttributeTask fieldId, 
    string alias)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldId | ExtendedAttributeTask | Указанный идентификатор поля [`ExtendedAttributeTask`](../../extendedattributetask/). |
| alias | Строка | Указанный строковый alias. |

### Возвращаемое значение

Создан экземпляр класса [`ExtendedAttributeDefinition`](../) с указанными *fieldId* и *alias*.

## Примеры

Используйте этот пример для создания пользовательского определения текстового поля:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

Показывает, как создать определение расширенного атрибута и установить строковое значение атрибута во время его создания.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My Text");
project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// создать расширенный атрибут со значением, равным 'Common Info'
var extendedAttribute = definition.CreateExtendedAttribute("Common Info");

// добавить расширенный атрибут, инициализированный значением 'Common Info'
task.ExtendedAttributes.Add(extendedAttribute);
```

### См. также

* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


