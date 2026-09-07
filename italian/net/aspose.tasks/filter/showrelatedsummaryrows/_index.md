---
title: "Filter.ShowRelatedSummaryRows"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Filter. Ottiene o imposta un valore che indica se le righe di riepilogo correlate sono visualizzate per il filtro"
type: docs
weight: 70
url: /it/net/aspose.tasks/filter/showrelatedsummaryrows/
---
## Filter.ShowRelatedSummaryRows property

Ottiene o imposta un valore che indica se le righe di riepilogo correlate sono visualizzate per il filtro.

```csharp
public bool ShowRelatedSummaryRows { get; set; }
```

## Esempi

Mostra come lavorare con i filtri.

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

// verifica i filtri delle risorse
List<Filter> resourceFilters = project.ResourceFilters.ToList();
Console.WriteLine("Project.ResourceFilters count: " + resourceFilters.Count);
Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + resourceFilters[0].FilterType);
Console.WriteLine("Resource filter ShowInMenu" + resourceFilters[0].ShowInMenu);
Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + resourceFilters[0].ShowRelatedSummaryRows);
```

### Vedi anche

* class [Filter](../)
* namespace [Aspose.Tasks](../../filter/)
* assembly [Aspose.Tasks](../../../)


