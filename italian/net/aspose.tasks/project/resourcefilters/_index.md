---
title: "Project.ResourceFilters"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Project. Ottiene tutte le definizioni di filtro basate sulle risorse. ResourceFilters è una collezione di oggetti Filter."
type: docs
weight: 760
url: /it/net/aspose.tasks/project/resourcefilters/
---
## Project.ResourceFilters property

Ottiene tutte le definizioni di filtro basate sulle risorse. ResourceFilters è una collezione di oggetti [`Filter`](../../filter/).

```csharp
public FilterCollection ResourceFilters { get; }
```

## Esempi

Mostra come leggere le definizioni di filtro attività/risorsa.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");
List<Filter> taskFilters = project.TaskFilters.ToList();
Console.WriteLine("Task Filters Count: " + taskFilters.Count);
Console.WriteLine("All Tasks: " + taskFilters[0].Name);
Console.WriteLine("Task Item: " + taskFilters[0].FilterType);
Console.WriteLine("Task Filters Show In Menu: " + taskFilters[0].ShowInMenu);
Console.WriteLine("Task filter ShowRelatedSummaryRows: " + taskFilters[0].ShowRelatedSummaryRows);

// Accedi ai filtri delle risorse
List<Filter> rscFilters = project.ResourceFilters.ToList();
Console.WriteLine("Project.ResourceFilters count: " + rscFilters.Count);
Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + rscFilters[0].FilterType);
Console.WriteLine("Resource filter ShowInMenu" + rscFilters[0].ShowInMenu);
Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + rscFilters[0].ShowRelatedSummaryRows);
```

### Vedi anche

* class [FilterCollection](../../filtercollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


