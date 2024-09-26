---
title: Project.ResourceFilters
second_title: Aspose.Tasks for .NET API Reference
description: Project property. Gets all the resourcebased filter definitions. ResourceFilters is a collection of Filter objects
type: docs
weight: 750
url: /net/aspose.tasks/project/resourcefilters/
---
## Project.ResourceFilters property

Gets all the resource-based filter definitions. ResourceFilters is a collection of [`Filter`](../../filter/) objects.

```csharp
public FilterCollection ResourceFilters { get; }
```

## Examples

Shows how to read task/resource filter definitions.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Filter> taskFilters = project.TaskFilters.ToList();
Console.WriteLine("Task Filters Count: " + taskFilters.Count);
Console.WriteLine("All Tasks: " + taskFilters[0].Name);
Console.WriteLine("Task Item: " + taskFilters[0].FilterType);
Console.WriteLine("Task Filters Show In Menu: " + taskFilters[0].ShowInMenu);
Console.WriteLine("Task filter ShowRelatedSummaryRows: " + taskFilters[0].ShowRelatedSummaryRows);

// Access resource filters
List<Filter> rscFilters = project.ResourceFilters.ToList();
Console.WriteLine("Project.ResourceFilters count: " + rscFilters.Count);
Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + rscFilters[0].FilterType);
Console.WriteLine("Resource filter ShowInMenu" + rscFilters[0].ShowInMenu);
Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + rscFilters[0].ShowRelatedSummaryRows);
```

### See Also

* class [FilterCollection](../../filtercollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


