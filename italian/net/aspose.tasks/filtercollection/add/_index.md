---
title: "FilterCollection.Add"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo FilterCollection. Aggiunge l'elemento specificato a questa collezione."
type: docs
weight: 30
url: /it/net/aspose.tasks/filtercollection/add/
---
## FilterCollection.Add method

Aggiunge l'elemento specificato a questa collezione.

```csharp
public void Add(Filter item)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| elemento | Filter | l'elemento specificato da aggiungere a questa collezione. |

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


