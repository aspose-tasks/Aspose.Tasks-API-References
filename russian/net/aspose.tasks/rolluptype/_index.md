---
title: "Перечисление RollupType"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.RollupType. Указывает тип свёртки"
type: docs
weight: 1950
url: /ru/net/aspose.tasks/rolluptype/
---
## RollupType enumeration

Указывает тип агрегирования.

```csharp
public enum RollupType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Null | `0` | Указывает тип свёртки Null. |
| Maximum | `1` | Указывает тип свёртки Maximum. |
| Minimum | `2` | Указывает тип свёртки Minimum. |
| Count | `3` | Указывает тип свёртки Count. |
| Sum | `4` | Указывает тип свёртки Sum. |
| Average | `5` | Указывает тип свёртки Average. |
| AverageFirstSublevel | `6` | Указывает тип свёртки Average First Sublevel. |
| CountFirstSublevel | `7` | Указывает тип свёртки Count First Sublevel. |
| CountNonsummaries | `8` | Указывает тип свёртки Count Non-Summaries. |

## Примеры

Показывает, как работать с типом расчёта расширенного определения атрибута.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 16, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// Создать определение атрибута с типом 'Formula', где значения для листовых задач и сводных задач вычисляются с помощью формулы.
var calculation = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date5, null);
calculation.CalculationType = CalculationType.Formula;
calculation.SummaryRowsCalculationType = SummaryRowsCalculationType.UseFormula;
calculation.Formula = "[stARt]";
project.ExtendedAttributes.Add(calculation);

// Создать определение атрибута, где значения для сводных задач вычисляются с использованием типа свёртки 'Average'.
var lookup = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Cost1, null);
lookup.SummaryRowsCalculationType = SummaryRowsCalculationType.Rollup;
lookup.RollupType = RollupType.Average;
project.ExtendedAttributes.Add(lookup);
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


