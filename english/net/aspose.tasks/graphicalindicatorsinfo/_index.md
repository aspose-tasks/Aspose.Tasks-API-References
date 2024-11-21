---
title: Class GraphicalIndicatorsInfo
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.GraphicalIndicatorsInfo class. Represents an graphical indicators definition associated with an extended attribute
type: docs
weight: 750
url: /net/aspose.tasks/graphicalindicatorsinfo/
---
## GraphicalIndicatorsInfo class

Represents an graphical indicators definition associated with an extended attribute.

```csharp
public sealed class GraphicalIndicatorsInfo
```

## Constructors

| Name | Description |
| --- | --- |
| [GraphicalIndicatorsInfo](graphicalindicatorsinfo/)() | Initializes a new instance of the `GraphicalIndicatorsInfo` type. |

## Properties

| Name | Description |
| --- | --- |
| [Criteria](../../aspose.tasks/graphicalindicatorsinfo/criteria/) { get; } | Gets a list of graphical indicator criteria. |
| [ProjectSummaryInheritFromNonSummaryRows](../../aspose.tasks/graphicalindicatorsinfo/projectsummaryinheritfromnonsummaryrows/) { get; set; } | Gets or sets flag indicating whether project summary row inherits criteria from summary rows. |
| [ShowDataValuesInTooltip](../../aspose.tasks/graphicalindicatorsinfo/showdatavaluesintooltip/) { get; set; } | Gets or sets flag indicating whether data values for the field should be shown in tooltips. |
| [SummaryRowsInheritFromNonSummaryRows](../../aspose.tasks/graphicalindicatorsinfo/summaryrowsinheritfromnonsummaryrows/) { get; set; } | Gets or sets flag indicating whether summary rows inherit criteria from nonsummary rows. |

## Examples

Shows how to set up graphical indicator for an extended attribute.

```csharp
Project project = new Project();

var def = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Number1, "Number field");
project.ExtendedAttributes.Add(def);
def.GraphicalIndicator = new GraphicalIndicatorsInfo();

GraphicalIndicatorCriteria criteria1 = new GraphicalIndicatorCriteria(
    GraphicalIndicatorCriteriaType.SummaryRows,
    FilterComparisonType.IsLessThan,
    2,
    new GraphicalIndicatorCriteriaValue(100m));

// 'IsWithin' criteria requires 2 values.
GraphicalIndicatorCriteria criteria2 = new GraphicalIndicatorCriteria(
    GraphicalIndicatorCriteriaType.SummaryRows,
    FilterComparisonType.IsWithin,
    4,
    new GraphicalIndicatorCriteriaValue(101),
    new GraphicalIndicatorCriteriaValue(1000m));

// 'IsAnyValue' criteria doesn't require values.
GraphicalIndicatorCriteria criteria3 = new GraphicalIndicatorCriteria(
    GraphicalIndicatorCriteriaType.SummaryRows,
    FilterComparisonType.IsAnyValue,
    4,
    null);

def.GraphicalIndicator.Criteria.Add(criteria1);
def.GraphicalIndicator.Criteria.Add(criteria2);
def.GraphicalIndicator.Criteria.Add(criteria3);

def.GraphicalIndicator.ProjectSummaryInheritFromNonSummaryRows = true;
def.GraphicalIndicator.SummaryRowsInheritFromNonSummaryRows = true;
def.GraphicalIndicator.ShowDataValuesInTooltip = false;

project.Save(OutDir + "CreateGraphicalIndicators_out.mpp", SaveFileFormat.Mpp);
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


