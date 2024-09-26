---
title: FilterCollection.CopyTo
second_title: Aspose.Tasks for .NET API Reference
description: FilterCollection method. Copies the elements of this collection to the specified array starting at the specified array index
type: docs
weight: 60
url: /net/aspose.tasks/filtercollection/copyto/
---
## FilterCollection.CopyTo method

Copies the elements of this collection to the specified array, starting at the specified array index.

```csharp
public void CopyTo(Filter[] array, int arrayIndex)
```

| Parameter | Type | Description |
| --- | --- | --- |
| array | Filter[] | the specified one-dimensional array to copy elements to |
| arrayIndex | Int32 | the zero-based index of the specified array at which copying begins. |

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

* class [Filter](../../filter/)
* class [FilterCollection](../)
* namespace [Aspose.Tasks](../../filtercollection/)
* assembly [Aspose.Tasks](../../../)


