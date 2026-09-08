---
title: "ExtendedAttributeDefinition.AddLookupValue"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ExtendedAttributeDefinition. Добавляет значение во внутренний список поиска. Это предпочтительный способ работы со списком ValueList"
type: docs
weight: 300
url: /ru/net/aspose.tasks/extendedattributedefinition/addlookupvalue/
---
## ExtendedAttributeDefinition.AddLookupValue method

Добавляет значение во внутренний список поиска. Это предпочтительный способ работы с [`ValueList`](../valuelist/).

```csharp
public void AddLookupValue(Value value)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| value | Значение | Значение для добавления в поиск. |

## Примечания

Этот метод работает только для экземпляров [`ExtendedAttributeDefinition`](../), у которых [`CalculationType`](../calculationtype/) равно Lookup.

## Примеры

Используйте этот код, чтобы добавить новое значение в список поиска:

```csharp
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
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

* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


