---
title: ExtendedAttributeDefinition.RollupType
second_title: Aspose.Tasks for .NET API Reference
description: ExtendedAttributeDefinition property. Gets or sets the way rollups are calculated
type: docs
weight: 230
url: /net/aspose.tasks/extendedattributedefinition/rolluptype/
---
## ExtendedAttributeDefinition.RollupType property

Gets or sets the way rollups are calculated.

```csharp
public RollupType RollupType { get; set; }
```

## Remarks

Writing currently supported for Xml format only.

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

* enum [RollupType](../../rolluptype/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


