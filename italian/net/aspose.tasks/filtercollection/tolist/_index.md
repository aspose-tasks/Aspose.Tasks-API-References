---
title: "FilterCollection.ToList"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo FilterCollection. Converte una collezione di filtri in un elenco di oggetti Filter"
type: docs
weight: 90
url: /it/net/aspose.tasks/filtercollection/tolist/
---
## FilterCollection.ToList method

Converte una collezione di filtri in un elenco di oggetti [`Filter`](../../filter/).

```csharp
public List<Filter> ToList()
```

### Valore di ritorno

Elenco generico di oggetti [`Filter`](../../filter/).

## Esempi

Mostra come lavorare con le collezioni di filtri.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");

// itera sui filtri delle attività
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

// itera sui filtri delle risorse
Console.WriteLine("Project.ResourceFilters count: " + project.ResourceFilters.Count);
foreach (var filter in project.ResourceFilters)
{
    Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + filter.FilterType);
    Console.WriteLine("Resource filter ShowInMenu" + filter.ShowInMenu);
    Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + filter.ShowRelatedSummaryRows);
}

var otherProject = new Project(DataDir + "Blank2010.mpp");

// cancella i filtri del progetto altrui
otherProject.TaskFilters.Clear();

// copia i filtri in un altro progetto
var filters = new Filter[project.TaskFilters.Count];
project.TaskFilters.CopyTo(filters, 0);

foreach (var filter in filters)
{
    otherProject.TaskFilters.Add(filter);
}

// aggiungi un filtro attività personalizzato
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

// rimuovi tutti i filtri
List<Filter> filtersToDelete = otherProject.TaskFilters.ToList();
foreach (var filter in filtersToDelete)
{
    otherProject.TaskFilters.Remove(filter);
}
```

### Vedi anche

* class [Filter](../../filter/)
* class [FilterCollection](../)
* namespace [Aspose.Tasks](../../filtercollection/)
* assembly [Aspose.Tasks](../../../)


