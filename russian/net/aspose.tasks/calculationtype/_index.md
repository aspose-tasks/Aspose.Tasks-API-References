---
title: "Перечисление CalculationType"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Aspose.Tasks.CalculationType enum. Указывает тип вычисления значения пользовательских атрибутов"
type: docs
weight: 220
url: /ru/net/aspose.tasks/calculationtype/
---
## CalculationType enumeration

Указывает тип расчёта значения пользовательского атрибута.

```csharp
public enum CalculationType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Означает, что расширенный атрибут не имеет таблицы поиска формул и просто сохраняет значение, установленное пользователем. |
| Lookup | `1` | Означает, что значение расширенного атрибута ограничено значениями из таблицы поиска. |
| Formula | `2` | Означает, что значение расширенного атрибута вычисляется с использованием формулы, определённой в [`Formula`](../extendedattributedefinition/formula/). |

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


