---
title: "ExtendedAttributeDefinition.CreateLookupTaskDefinition"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ExtendedAttributeDefinition. Фабричный метод, который создает определение расширенного атрибута с поиском. У него CalculationType равно Lookup и может использоваться только в Tasks. Требуется указать fieldId и alias при вызове этого метода. Тип поля выводится из идентификатора поля."
type: docs
weight: 20
url: /ru/net/aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/
---
## CreateLookupTaskDefinition(ExtendedAttributeTask, string) {#createlookuptaskdefinition_1}

Фабричный метод, который создает определение расширенного атрибута с поиском. У него [`CalculationType`](../calculationtype/) равно Lookup и может использоваться только в Tasks. Требуется указать *fieldId* и *alias* при вызове этого метода. Тип поля выводится из идентификатора поля.

```csharp
public static ExtendedAttributeDefinition CreateLookupTaskDefinition(ExtendedAttributeTask fieldId, 
    string alias)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fieldId | ExtendedAttributeTask | Указанный идентификатор поля [`ExtendedAttributeTask`](../../extendedattributetask/). |
| alias | Строка | Указанный строковый alias. |

### Возвращаемое значение

Создан экземпляр класса [`ExtendedAttributeDefinition`](../) с указанными *fieldId* и *alias*.

## Примеры

Используйте этот пример, чтобы создать определение пользовательского поля для задачи с поиском, а затем заполнить его текстовыми значениями:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Text27, "My custom field");
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
taskTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(taskTextAttr);
```

Показывает, как записать обновленные определения расширенных атрибутов.

```csharp
var project = new Project(DataDir + "WriteUpdatedExtendedAttributeDefinitions.mpp");

// Добавить новый расширенный атрибут text3 с lookup и одним значением lookup.
var definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Text3, "New text3 attribute");
definition.ElementType = ElementType.Task;
project.ExtendedAttributes.Add(definition);

var textVal = new Value
{
    Id = 1,
    Description = "Text value descr",
    Val = "Text value1"
};

definition.AddLookupValue(textVal);

// Добавить новый расширенный атрибут cost1 с lookup и двумя значениями стоимости.
var taskCostAttributeDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Cost1, "New cost1 attribute");
project.ExtendedAttributes.Add(taskCostAttributeDefinition);

var costVal1 = new Value
{
    Id = 2,
    Description = "Cost value 1 descr",
    Val = "99900"
};

var costVal2 = new Value
{
    Id = 3,
    Description = "Cost value 2 descr",
    Val = "11100"
};

taskCostAttributeDefinition.AddLookupValue(costVal1);
taskCostAttributeDefinition.AddLookupValue(costVal2);

// Добавить новую задачу и назначить значение lookup атрибута.
var task = project.RootTask.Children.Add("New task");

var taskAttr = taskCostAttributeDefinition.CreateExtendedAttribute(costVal1);
task.ExtendedAttributes.Add(taskAttr);

var taskStartAttributeDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Start7, "New start 7 attribute");

var startVal = new Value
{
    Id = 4,
    DateTimeValue = DateTime.Now,
    Description = "Start 7 value description"
};

taskStartAttributeDefinition.AddLookupValue(startVal);

project.ExtendedAttributes.Add(taskStartAttributeDefinition);

var taskFinishAttributeDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Finish4, "New finish 4 attribute");

var finishVal = new Value
{
    Id = 5,
    DateTimeValue = DateTime.Now,
    Description = "Finish 4 value description"
};

taskFinishAttributeDefinition.ValueList.Add(finishVal);

project.ExtendedAttributes.Add(taskFinishAttributeDefinition);

var numberAttributeDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Number20, "New number attribute");

var val1 = new Value
{
    Id = 6,
    Val = "1",
    Description = "Number 1 value"
};
var val2 = new Value
{
    Id = 7,
    Val = "2",
    Description = "Number 2 value"
};
var val3 = new Value();
val2.Id = 8;
val3.Val = "3";
val3.Description = "Number 3 value";

numberAttributeDefinition.AddLookupValue(val1);
numberAttributeDefinition.AddLookupValue(val2);
numberAttributeDefinition.AddLookupValue(val3);

project.ExtendedAttributes.Add(numberAttributeDefinition);

var rscStartAttributeDefinition = ExtendedAttributeDefinition.CreateLookupResourceDefinition(ExtendedAttributeResource.Start5, "New start5 attribute");

var value = new Value
{
    Id = 9,
    DateTimeValue = DateTime.Now,
    Description = "this is start5 value descr"
};

rscStartAttributeDefinition.AddLookupValue(value);

project.ExtendedAttributes.Add(rscStartAttributeDefinition);

// Определить атрибут длительности без lookup.
var taskDurationAttributeDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Duration1, "New Duration");
project.ExtendedAttributes.Add(taskDurationAttributeDefinition);

// Добавить новую задачу и назначить значение длительности ранее определённому атрибуту длительности.
var timeTask = project.RootTask.Children.Add("New task");

var durationExtendedAttribute = taskDurationAttributeDefinition.CreateExtendedAttribute();

durationExtendedAttribute.DurationValue = project.GetDuration(3.0, TimeUnitType.Hour);
timeTask.ExtendedAttributes.Add(durationExtendedAttribute);

var options = new MPPSaveOptions
{
    WriteViewData = true
};

project.Save(OutDir + "WriteUpdatedExtendedAttributeDefinitions_out.mpp", options);
```

### См. также

* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateLookupTaskDefinition(CustomFieldType, ExtendedAttributeTask, string) {#createlookuptaskdefinition}

Фабричный метод, который создает определение расширенного атрибута с поиском. У него [`CalculationType`](../calculationtype/) равно Lookup и может использоваться только в Tasks. Требуется указать *customFieldType*, *fieldId* и *alias* при вызове этого метода.

```csharp
public static ExtendedAttributeDefinition CreateLookupTaskDefinition(
    CustomFieldType customFieldType, ExtendedAttributeTask fieldId, string alias)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| customFieldType | CustomFieldType | Указанный тип [`CustomFieldType`](../../customfieldtype/). |
| fieldId | ExtendedAttributeTask | Указанный идентификатор поля [`ExtendedAttributeTask`](../../extendedattributetask/). |
| alias | Строка | Указанный строковый alias. |

### Возвращаемое значение

Создан экземпляр класса [`ExtendedAttributeDefinition`](../) с указанными *customFieldType*, *fieldId* и *alias*.

## Примеры

Используйте этот пример, чтобы создать определение пользовательского поля для задачи с поиском, а затем заполнить его текстовыми значениями:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text27, "My custom field");
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
taskTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(taskTextAttr);
```

Показывает, как добавить расширенные атрибуты с выпадающими списками для назначений.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Назначьте ресурс "1 TRG: Trade Group" задаче "TASK 1", создав объект ResourceAssignment.
var resource = project.Resources.GetById(1);
var task = project.RootTask.Children.GetById(1);
var assignment = project.ResourceAssignments.Add(task, resource);

// Создайте определение пользовательского атрибута с выпадающим списком.
var resExtendedAttributeDefinition = ExtendedAttributeDefinition.CreateLookupResourceDefinition(
    CustomFieldType.Cost,
    ExtendedAttributeResource.Cost5,
    "My lookup resource cost");
project.ExtendedAttributes.Add(resExtendedAttributeDefinition);

var firstValue = new Value { NumericValue = 1500, Description = "Val 1", Id = 1, Val = "1500" };
var secondValue = new Value { NumericValue = 2500, Description = "Val 2", Id = 2 };
resExtendedAttributeDefinition.AddLookupValue(firstValue);
resExtendedAttributeDefinition.AddLookupValue(secondValue);

// Это значение можно увидеть в представлении "Resource usage" в MS Project.
var attributeValue = resExtendedAttributeDefinition.CreateExtendedAttribute(firstValue);
assignment.ExtendedAttributes.Add(attributeValue);

// Создайте определение пользовательского атрибута с выпадающим списком.
var taskCostAttr = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost4, "My lookup task cost");
project.ExtendedAttributes.Add(taskCostAttr);
var taskFirstValue = new Value { NumericValue = 18, Description = "Task val 1", Id = 3, Val = "18" };
var resSecondValue = new Value { NumericValue = 30, Description = "Task val 2", Id = 4 };
var taskWrongValue = new Value { NumericValue = 99, Description = "Task val Wrong", Id = 5, Val = "18" };

taskCostAttr.AddLookupValue(taskFirstValue);
resExtendedAttributeDefinition.AddLookupValue(resSecondValue);

// Это значение можно увидеть в представлении "Task usage" в MS Project.
assignment.ExtendedAttributes.Add(taskCostAttr.CreateExtendedAttribute(taskFirstValue));

// Неправильные значения могут быть удалены позже
taskCostAttr.RemoveLookupValue(taskWrongValue);

// Работа с проектом...
```

### См. также

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


