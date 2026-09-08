---
title: "ExtendedAttributeDefinition.SummaryRowsCalculationType"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство ExtendedAttributeDefinition. Возвращает или задает тип расчёта значения пользовательских атрибутов для строк итогов"
type: docs
weight: 260
url: /ru/net/aspose.tasks/extendedattributedefinition/summaryrowscalculationtype/
---
## ExtendedAttributeDefinition.SummaryRowsCalculationType property

Получает или задает тип расчёта значения пользовательского атрибута для строк итогов.

```csharp
public SummaryRowsCalculationType SummaryRowsCalculationType { get; set; }
```

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

* enum [SummaryRowsCalculationType](../../summaryrowscalculationtype/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


