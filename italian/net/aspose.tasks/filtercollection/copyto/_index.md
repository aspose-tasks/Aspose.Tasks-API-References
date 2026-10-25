---
title: "FilterCollection.CopyTo"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo FilterCollection. Copia gli elementi di questa collezione nell'array specificato a partire dall'indice specificato dell'array"
type: docs
weight: 60
url: /it/net/aspose.tasks/filtercollection/copyto/
---
## FilterCollection.CopyTo method

Copia gli elementi di questa collezione nell'array specificato, a partire dall'indice dell'array specificato.

```csharp
public void CopyTo(Filter[] array, int arrayIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| array | Filter[] | l'array monodimensionale specificato a cui copiare gli elementi |
| arrayIndex | Int32 | l'indice basato su zero dell'array specificato al quale inizia la copia. |

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


