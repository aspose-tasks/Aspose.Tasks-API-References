---
title: "ExtendedAttribute.AttributeDefinition"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство ExtendedAttribute. Возвращает определение атрибута"
type: docs
weight: 10
url: /ru/net/aspose.tasks/extendedattribute/attributedefinition/
---
## ExtendedAttribute.AttributeDefinition property

Получает определение атрибута.

```csharp
public ExtendedAttributeDefinition AttributeDefinition { get; }
```

## Примеры

Показывает, как изменить определение атрибута расширенного атрибута.

```csharp
var project = new Project();

// создать новое определение расширенного атрибута задачи
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost1, string.Empty);

// добавьте формулу к атрибуту.
definition.Alias = "Difference between Cost and Actual Cost";
definition.Formula = "[Cost]-[Actual Cost]";

project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 21, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task.Set(Tsk.Finish, new DateTime(2020, 4, 21, 17, 0, 0));
task.Set(Tsk.Deadline, new DateTime(2020, 4, 22, 17, 0, 0));
task.Set(Tsk.Cost, 20);
task.Set(Tsk.ActualCost, 13);

// создать расширенный атрибут
var extendedAttribute = definition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(extendedAttribute);

Console.WriteLine("Before change:");
Console.WriteLine("Alias: " + definition.Alias);
Console.WriteLine("Field Id: " + extendedAttribute.FieldId);
Console.WriteLine("Value: " + extendedAttribute.NumericValue);

// создать новое определение расширенного атрибута даты
var newDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Date, ExtendedAttributeTask.Date1, string.Empty);

// добавьте формулу к атрибуту.
newDefinition.Alias = "Days from finish to deadline";
newDefinition.Formula = "[Deadline] - [Finish]";
project.ExtendedAttributes.Add(newDefinition);

extendedAttribute = newDefinition.CreateExtendedAttribute();

Console.WriteLine();
Console.WriteLine("After change:");
Console.WriteLine("Alias: " + definition.Alias);
Console.WriteLine("Field Id: " + extendedAttribute.FieldId);
Console.WriteLine("Value: " + extendedAttribute.DateValue.Day);
```

### См. также

* class [ExtendedAttributeDefinition](../../extendedattributedefinition/)
* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


