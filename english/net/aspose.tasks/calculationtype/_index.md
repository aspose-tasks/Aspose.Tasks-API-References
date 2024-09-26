---
title: Enum CalculationType
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.CalculationType enum. Specifies the type of a calculation of the custom attributes value
type: docs
weight: 220
url: /net/aspose.tasks/calculationtype/
---
## CalculationType enumeration

Specifies the type of a calculation of the custom attribute's value.

```csharp
public enum CalculationType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| None | `0` | Means the extended attribute has no lookup table of formula and simply stores value set by the user. |
| Lookup | `1` | Means the value of the extended attribute is restricted to values from a lookup table. |
| Formula | `2` | Means the value of the extended attribute is calculated using formula defined in [`Formula`](../extendedattributedefinition/formula/). |

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


