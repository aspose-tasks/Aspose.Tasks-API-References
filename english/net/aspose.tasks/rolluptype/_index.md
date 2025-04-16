---
title: Enum RollupType
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.RollupType enum. Specifies the rollup type
type: docs
weight: 1890
url: /net/aspose.tasks/rolluptype/
---
## RollupType enumeration

Specifies the rollup type.

```csharp
public enum RollupType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Null | `0` | Indicates Null rollup type. |
| Maximum | `1` | Indicates Maximum rollup type. |
| Minimum | `2` | Indicates Minimum rollup type. |
| Count | `3` | Indicates Count rollup type. |
| Sum | `4` | Indicates Sum rollup type. |
| Average | `5` | Indicates Average rollup type. |
| AverageFirstSublevel | `6` | Indicates Average First Sublevel rollup type. |
| CountFirstSublevel | `7` | Indicates Count First Sublevel rollup type. |
| CountNonsummaries | `8` | Indicates Count Non-Summaries rollup type. |

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


