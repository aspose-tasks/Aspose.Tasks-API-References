---
title: "ExtendedAttribute.FlagValue"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство ExtendedAttribute. Получает или задает значение, указывающее, установлен ли флаг для атрибута типа Flag"
type: docs
weight: 50
url: /ru/net/aspose.tasks/extendedattribute/flagvalue/
---
## ExtendedAttribute.FlagValue property

Получает или задает значение, указывающее, установлен ли флаг для атрибута типа 'Flag'.

```csharp
public bool FlagValue { get; set; }
```

### Исключения

| исключение | условие |
| --- | --- |
| InvalidOperationException | Выбрасывается, если свойство [`AttributeDefinition`](../attributedefinition/) не инициализировано или текущий атрибут не является флаговым атрибутом. |

## Примеры

Показывает, как создать логический расширенный атрибут.

```csharp
var project = new Project();

// создать новое определение расширенного атрибута задачи
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Flag, ExtendedAttributeTask.Flag1, "Is Finished");

// добавьте формулу к атрибуту.
definition.Formula = "[% Complete] = 100";

project.ExtendedAttributes.Add(definition);

var finished = project.RootTask.Children.Add("Task");
finished.Set(Tsk.Start, new DateTime(2020, 4, 21, 8, 0, 0));
finished.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
finished.Set(Tsk.Finish, new DateTime(2020, 4, 21, 17, 0, 0));
finished.Set(Tsk.ActualStart, new DateTime(2020, 4, 21, 8, 0, 0));
finished.Set(Tsk.ActualDuration, project.GetDuration(1, TimeUnitType.Day));
finished.Set(Tsk.ActualFinish, new DateTime(2020, 4, 21, 17, 0, 0));
finished.Set(Tsk.PercentComplete, 100);

var running = project.RootTask.Children.Add("Task");
running.Set(Tsk.Start, new DateTime(2020, 4, 21, 8, 0, 0));
running.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
running.Set(Tsk.Finish, new DateTime(2020, 4, 21, 17, 0, 0));
running.Set(Tsk.ActualStart, new DateTime(2020, 4, 21, 8, 0, 0));

Console.WriteLine(running.Get(Tsk.PercentComplete));
// создать расширенный атрибут
var runningFlagAttribute = definition.CreateExtendedAttribute();
var finishedFlagAttribute = definition.CreateExtendedAttribute();
running.ExtendedAttributes.Add(runningFlagAttribute);
finished.ExtendedAttributes.Add(finishedFlagAttribute);

Console.WriteLine("Alias: {0}\n", definition.Alias);
Console.WriteLine("(Finished Task) Field Id: " + finishedFlagAttribute.FieldId);
Console.WriteLine("(Finished Task) Value: {0}\n", finishedFlagAttribute.FlagValue);
Console.WriteLine("(Running Task) Field Id: " + runningFlagAttribute.FieldId);
Console.WriteLine("(Running Task) Value: " + runningFlagAttribute.FlagValue);
```

### См. также

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


