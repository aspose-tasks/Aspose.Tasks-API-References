---
title: Class FilterCollection
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.FilterCollection class. Contains a list of Filter objects. Implements ICollectionFilter interface
type: docs
weight: 610
url: /net/aspose.tasks/filtercollection/
---
## FilterCollection class

Contains a list of [`Filter`](../filter/) objects. Implements ICollection&lt;Filter&gt; interface.

```csharp
public class FilterCollection : ICollection<Filter>
```

## Properties

| Name | Description |
| --- | --- |
| [Count](../../aspose.tasks/filtercollection/count/) { get; } | Gets the number of elements contained in this collection. |
| [IsReadOnly](../../aspose.tasks/filtercollection/isreadonly/) { get; } | Gets a value indicating whether this collection is read-only; otherwise, false. |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.tasks/filtercollection/add/)(Filter) | Adds the specified item to this collection. |
| [Clear](../../aspose.tasks/filtercollection/clear/)() | Removes all items from this collection. |
| [Contains](../../aspose.tasks/filtercollection/contains/)(Filter) | Returns true if the specified item is found in this collection; otherwise, false. |
| [CopyTo](../../aspose.tasks/filtercollection/copyto/)(Filter[], int) | Copies the elements of this collection to the specified array, starting at the specified array index. |
| [GetEnumerator](../../aspose.tasks/filtercollection/getenumerator/)() | Returns an enumerator for this collection. |
| [Remove](../../aspose.tasks/filtercollection/remove/)(Filter) | Removes the first occurrence of a specific object from this collection. |
| [ToList](../../aspose.tasks/filtercollection/tolist/)() | Converts a filter collection to a list of [`Filter`](../filter/) objects. |

## Examples

Shows how to work with filter collections.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");

// iterate over task filters
Console.WriteLine("Print task filters of {0} project: ", project.Get(Prj.Name));
Console.WriteLine("Task Filters Count: " + project.TaskFilters.Count);
foreach (var filter in project.TaskFilters)
{
    Console.WriteLine("All Tasks: " + filter.Name);
    Console.WriteLine("Task Item: " + filter.FilterType);
    Console.WriteLine("Task Filters Show In Menu: " + filter.ShowInMenu);
    Console.WriteLine("Task filter ShowRelatedSummaryRows: " + filter.ShowRelatedSummaryRows);
    Console.WriteLine();
}

// iterate over resource filters
Console.WriteLine("Project.ResourceFilters count: " + project.ResourceFilters.Count);
foreach (var filter in project.ResourceFilters)
{
    Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + filter.FilterType);
    Console.WriteLine("Resource filter ShowInMenu" + filter.ShowInMenu);
    Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + filter.ShowRelatedSummaryRows);
}

var otherProject = new Project(DataDir + "Blank2010.mpp");

// clear other project's filters
otherProject.TaskFilters.Clear();

// copy filters to other project
var filters = new Filter[project.TaskFilters.Count];
project.TaskFilters.CopyTo(filters, 0);

foreach (var filter in filters)
{
    otherProject.TaskFilters.Add(filter);
}

// add custom task filter
var customFilter = new Filter();
customFilter.Name = "Custom Filter";
customFilter.ShowInMenu = true;
customFilter.ShowRelatedSummaryRows = true;

if (!otherProject.TaskFilters.Contains(customFilter))
{
    if (!otherProject.TaskFilters.IsReadOnly)
    {
        otherProject.TaskFilters.Add(customFilter);
    }
}

// remove all filters
List<Filter> filtersToDelete = otherProject.TaskFilters.ToList();
foreach (var filter in filtersToDelete)
{
    otherProject.TaskFilters.Remove(filter);
}
```

### See Also

* class [Filter](../filter/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


