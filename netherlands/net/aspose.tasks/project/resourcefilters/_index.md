---
title: "Project.ResourceFilters"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Project-eigenschap. Haalt alle op resource gebaseerde filterdefinities op. ResourceFilters is een collectie van Filter-objecten."
type: docs
weight: 760
url: /nl/net/aspose.tasks/project/resourcefilters/
---
## Project.ResourceFilters property

Haalt alle resource-gebaseerde filterdefinities op. ResourceFilters is een collectie van [`Filter`](../../filter/) objecten.

```csharp
public FilterCollection ResourceFilters { get; }
```

## Voorbeelden

Toont hoe taak/resource-filterdefinities te lezen.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Filter> taskFilters = project.TaskFilters.ToList();
Console.WriteLine("Task Filters Count: " + taskFilters.Count);
Console.WriteLine("All Tasks: " + taskFilters[0].Name);
Console.WriteLine("Task Item: " + taskFilters[0].FilterType);
Console.WriteLine("Task Filters Show In Menu: " + taskFilters[0].ShowInMenu);
Console.WriteLine("Task filter ShowRelatedSummaryRows: " + taskFilters[0].ShowRelatedSummaryRows);

// Toegang tot resource-filters
List<Filter> rscFilters = project.ResourceFilters.ToList();
Console.WriteLine("Project.ResourceFilters count: " + rscFilters.Count);
Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + rscFilters[0].FilterType);
Console.WriteLine("Resource filter ShowInMenu" + rscFilters[0].ShowInMenu);
Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + rscFilters[0].ShowRelatedSummaryRows);
```

### Zie ook

* class [FilterCollection](../../filtercollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


