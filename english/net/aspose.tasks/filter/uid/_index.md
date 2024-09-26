---
title: Filter.Uid
second_title: Aspose.Tasks for .NET API Reference
description: Filter property. Gets the unique identifier of a filter
type: docs
weight: 80
url: /net/aspose.tasks/filter/uid/
---
## Filter.Uid property

Gets the unique identifier of a filter.

```csharp
public int Uid { get; }
```

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

* class [Filter](../)
* namespace [Aspose.Tasks](../../filter/)
* assembly [Aspose.Tasks](../../../)


