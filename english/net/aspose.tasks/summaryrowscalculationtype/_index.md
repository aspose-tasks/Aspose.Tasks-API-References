---
title: Enum SummaryRowsCalculationType
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.SummaryRowsCalculationType enum. Specifies the type of a calculation of the custom attributes value for summary rows
type: docs
weight: 2280
url: /net/aspose.tasks/summaryrowscalculationtype/
---
## SummaryRowsCalculationType enumeration

Specifies the type of a calculation of the custom attribute's value for summary rows.

```csharp
public enum SummaryRowsCalculationType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| None | `0` | Means the custom attribute's value for summary rows is not calculated. |
| Rollup | `1` | Means the custom attribute's value for summary rows is calculated using rollup function defined in [`RollupType`](../extendedattributedefinition/rolluptype/). |
| UseFormula | `2` | Means the custom attribute's value for summary rows is calculated using formula defined in [`Formula`](../extendedattributedefinition/formula/). |

## Examples

Shows how to work with calculation type of an extended attribute definition.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 16, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// create attribute definition with 'Formula' type where values for leaf tasks and summary tasks are calculated using formula.
var calculation = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date5, null);
calculation.CalculationType = CalculationType.Formula;
calculation.SummaryRowsCalculationType = SummaryRowsCalculationType.UseFormula;
calculation.Formula = "[stARt]";
project.ExtendedAttributes.Add(calculation);

// create attribute definition where values for summary tasks are calculated using 'Average' rollup type.
var lookup = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Cost1, null);
lookup.SummaryRowsCalculationType = SummaryRowsCalculationType.Rollup;
lookup.RollupType = RollupType.Average;
project.ExtendedAttributes.Add(lookup);
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


