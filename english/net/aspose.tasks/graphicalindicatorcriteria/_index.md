---
title: Class GraphicalIndicatorCriteria
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.GraphicalIndicatorCriteria class. Represents one graphical indicator criteria associated with an extended attribute
type: docs
weight: 720
url: /net/aspose.tasks/graphicalindicatorcriteria/
---
## GraphicalIndicatorCriteria class

Represents one graphical indicator criteria associated with an extended attribute.

```csharp
public sealed class GraphicalIndicatorCriteria
```

## Constructors

| Name | Description |
| --- | --- |
| [GraphicalIndicatorCriteria](graphicalindicatorcriteria/#constructor)(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue) | Initializes a new instance of the `GraphicalIndicatorCriteria` type. |
| [GraphicalIndicatorCriteria](graphicalindicatorcriteria/#constructor_1)(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue, GraphicalIndicatorCriteriaValue) | Initializes a new instance of the `GraphicalIndicatorCriteria` type. |

## Properties

| Name | Description |
| --- | --- |
| [ImageIndex](../../aspose.tasks/graphicalindicatorcriteria/imageindex/) { get; } | Gets the index of the image to display when the field meets the criteria. |
| [RowType](../../aspose.tasks/graphicalindicatorcriteria/rowtype/) { get; } | Gets the value of [`GraphicalIndicatorCriteriaType`](../graphicalindicatorcriteriatype/) enum which denotes for which rows the indicator is applied. |
| [Test](../../aspose.tasks/graphicalindicatorcriteria/test/) { get; } | Gets the type of comparison made between extended attribute's value and Values that acts as a criteria for the application of the graphical indicator. [`FilterComparisonType`](../filtercomparisontype/) |
| [Value1](../../aspose.tasks/graphicalindicatorcriteria/value1/) { get; } | Gets the value used to test extended attribute's value. |
| [Value2](../../aspose.tasks/graphicalindicatorcriteria/value2/) { get; } | Gets the second value used to test extended attribute's value in case of 'IsWithin' and 'IsNotWithin' comparison types. |

## Methods

| Name | Description |
| --- | --- |
| override [ToString](../../aspose.tasks/graphicalindicatorcriteria/tostring/)() | Returns string representation of the instance of the `GraphicalIndicatorCriteria` class. |

## Examples

Shows how to retrieve graphical indicators info.

```csharp
Project project = new Project(DataDir + "graphical_indicators.mpp");

foreach (var ea in project.ExtendedAttributes)
{
    if (ea.GraphicalIndicator == null)
    {
        continue;
    }

    Console.WriteLine("GI for field '{0}':", ea.FieldName);

    foreach (var criterion in ea.GraphicalIndicator.Criteria)
    {
        Console.WriteLine("Row type: {0}", criterion.RowType);
        Console.WriteLine("Image index: {0}", criterion.ImageIndex);
        Console.Write(criterion.Test);
        if (criterion.Value1 != null)
        {
            Console.Write(" ");
            Console.Write(criterion.Value1.RawValue);
        }

        if (criterion.Value2 != null)
        {
            Console.Write(" ");
            Console.WriteLine(criterion.Value2.RawValue);
        }

        Console.WriteLine();
    }
}
```

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


