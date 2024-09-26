---
title: Class Filter
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Filter class. Represents a filter in Project
type: docs
weight: 600
url: /net/aspose.tasks/filter/
---
## Filter class

Represents a filter in Project.

```csharp
public sealed class Filter : IComparable<Filter>, IEquatable<Filter>
```

## Constructors

| Name | Description |
| --- | --- |
| [Filter](filter/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [Criteria](../../aspose.tasks/filter/criteria/) { get; set; } | Gets or sets the criteria that tasks or resources must meet to be displayed in MSP view. |
| [FilterType](../../aspose.tasks/filter/filtertype/) { get; set; } | Gets the type of the filter. |
| [Index](../../aspose.tasks/filter/index/) { get; } | Gets the index of a `Filter` object in the Filters containing object. |
| [Name](../../aspose.tasks/filter/name/) { get; set; } | Gets or sets the name of a Filter object. |
| [ShowInMenu](../../aspose.tasks/filter/showinmenu/) { get; set; } | Gets or sets a value indicating whether project shows the filter name in the Filter drop-down list on the View tab of the Ribbon. |
| [ShowRelatedSummaryRows](../../aspose.tasks/filter/showrelatedsummaryrows/) { get; set; } | Gets or sets a value indicating whether related summary rows are displayed for the filter. |
| [Uid](../../aspose.tasks/filter/uid/) { get; } | Gets the unique identifier of a filter. |

## Methods

| Name | Description |
| --- | --- |
| [CompareTo](../../aspose.tasks/filter/compareto/)(Filter) | Compares this instance to the specified instance of the `Filter` class and returns an indication of their relative order. |
| [Equals](../../aspose.tasks/filter/equals/#equals)(Filter) | Returns a value indicating whether this instance is equal to the specified AssignmentBaseline object. |
| override [Equals](../../aspose.tasks/filter/equals/#equals_1)(object) | Returns a value indicating whether this instance is equal to the specified AssignmentBaseline object. |
| override [GetHashCode](../../aspose.tasks/filter/gethashcode/)() | Returns a hash code value for the filter. |
| [operator ==](../../aspose.tasks/filter/op_equality/) | Returns a value indicating whether this instance is equal to a specified object. |
| [operator &gt;](../../aspose.tasks/filter/op_greaterthan/) | Returns a value indicating whether this instance is greater than a specified object. |
| [operator &gt;=](../../aspose.tasks/filter/op_greaterthanorequal/) | Returns a value indicating whether this instance is greater than or equal to a specified object. |
| [operator !=](../../aspose.tasks/filter/op_inequality/) | Returns a value indicating whether this instance is not equal to a specified object. |
| [operator &lt;](../../aspose.tasks/filter/op_lessthan/) | Returns a value indicating whether this instance is less than a specified object. |
| [operator &lt;=](../../aspose.tasks/filter/op_lessthanorequal/) | Returns a value indicating whether this instance is less than or equal to a specified object. |

## Examples

Shows how to work with filters.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Filter> filters = project.TaskFilters.ToList();
Console.WriteLine("Task filters count: " + filters.Count);
foreach (var filter in filters)
{
    Console.WriteLine("Uid: " + filter.Uid);
    Console.WriteLine("Index: " + filter.Index);
    Console.WriteLine("Name: " + filter.Name);
    Console.WriteLine("Type: " + filter.FilterType);
    Console.WriteLine("Show In Menu: " + filter.ShowInMenu);
    Console.WriteLine("Show Related Summary Rows: " + filter.ShowRelatedSummaryRows);
}

// check resource filters
List<Filter> resourceFilters = project.ResourceFilters.ToList();
Console.WriteLine("Project.ResourceFilters count: " + resourceFilters.Count);
Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + resourceFilters[0].FilterType);
Console.WriteLine("Resource filter ShowInMenu" + resourceFilters[0].ShowInMenu);
Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + resourceFilters[0].ShowRelatedSummaryRows);
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


