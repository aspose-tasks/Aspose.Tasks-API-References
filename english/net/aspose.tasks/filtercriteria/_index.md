---
title: Class FilterCriteria
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.FilterCriteria class. Defines the criteria that tasks or resources must meet to be displayed in MSP view
type: docs
weight: 630
url: /net/aspose.tasks/filtercriteria/
---
## FilterCriteria class

Defines the criteria that tasks or resources must meet to be displayed in MSP view.

```csharp
public class FilterCriteria
```

## Constructors

| Name | Description |
| --- | --- |
| [FilterCriteria](filtercriteria/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [CriteriaRows](../../aspose.tasks/filtercriteria/criteriarows/) { get; } | Gets the list of child `FilterCriteria` rows. If the filter contains more than one criterion row then the effect of an And operator is that the criteria for both rows must be met for the task or resource to be displayed as a result of this filter. The effect of an Or operator is that the criteria for one or the other row must be met. |
| [Field](../../aspose.tasks/filtercriteria/field/) { get; set; } | Gets or sets a [`Field`](./field/) to change. |
| [Operation](../../aspose.tasks/filtercriteria/operation/) { get; set; } | Gets or sets the criterion established with FieldName, Test, and Value relates to other criteria in the filter. |
| [Test](../../aspose.tasks/filtercriteria/test/) { get; set; } | Gets or sets the type of comparison made between FieldName and Value that acts as selection criteria for the filter. [`FilterComparisonType`](../filtercomparisontype/) |
| [Values](../../aspose.tasks/filtercriteria/values/) { get; } | Gets the object values to compare with the value of the field specified with FieldName. |

## Methods

| Name | Description |
| --- | --- |
| [IsFieldValue](../../aspose.tasks/filtercriteria/isfieldvalue/)() | Gets whether the right-hand value of FilterCriteria is a field reference, not a constant value. |
| [SetValueField](../../aspose.tasks/filtercriteria/setvaluefield/)(Field) | Sets the field whose value will be compared with the value of the field specified by FieldName. |
| override [ToString](../../aspose.tasks/filtercriteria/tostring/)() | Returns string representation of the instance of the `FilterCriteria` class. |

## Examples

Shows how to read task filter criteria.

```csharp
var project = new Project(DataDir + "Project2003.mpp");

var filter = project.TaskFilters.ToList()[1];
Console.WriteLine("Count of criteria rows: " + filter.Criteria.CriteriaRows.Count);
foreach (var row in filter.Criteria.CriteriaRows)
{
    Console.WriteLine("Field: " + row.Field);
    Console.WriteLine("Operation: " + row.Operation);
    Console.WriteLine("Test: " + row.Test);

    var values = row.Values.Where(c => c != null).ToArray();
    if (values.Length == 0)
    {
        continue;
    }

    Console.WriteLine("Value{0}: {1}", values.Length == 1 ? "" : "s", string.Join(", ", values));
}

// print filter criteria as a string 
Console.WriteLine(filter.Criteria.Operation.ToString());

var criteria1 = filter.Criteria.CriteriaRows[0];
Console.WriteLine("Criteria filter 1:");
Console.WriteLine(criteria1.ToString());

var criteria2 = filter.Criteria.CriteriaRows[1];
Console.WriteLine(criteria2.Operation.ToString());
Console.WriteLine(criteria2.CriteriaRows.Count);
Console.WriteLine("Criteria filter 2:");
Console.WriteLine(criteria2.ToString());

var criteria21 = criteria2.CriteriaRows[0];
Console.WriteLine("Criteria filter 21:");
Console.WriteLine(criteria21.ToString());

var criteria22 = criteria2.CriteriaRows[1];
Console.WriteLine("Criteria filter 22:");
Console.WriteLine(criteria22.ToString());
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


