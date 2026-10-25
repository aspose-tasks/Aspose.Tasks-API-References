---
title: "Classe FilterCollection"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.FilterCollection classe. Contiene un elenco di oggetti Filter. Implementa l'interfaccia ICollectionFilter."
type: docs
weight: 610
url: /it/net/aspose.tasks/filtercollection/
---
## FilterCollection class

Contiene un elenco di oggetti [`Filter`](../filter/) . Implementa l'interfaccia ICollection&lt;Filter&gt;.

```csharp
public class FilterCollection : ICollection<Filter>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.tasks/filtercollection/count/) { get; } | Ottiene il numero di elementi contenuti in questa collezione. |
| [IsReadOnly](../../aspose.tasks/filtercollection/isreadonly/) { get; } | Restituisce un valore che indica se questa collezione è di sola lettura; altrimenti, false. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.tasks/filtercollection/add/)(Filter) | Aggiunge l'elemento specificato a questa collezione. |
| [Clear](../../aspose.tasks/filtercollection/clear/)() | Rimuove tutti gli elementi da questa collezione. |
| [Contains](../../aspose.tasks/filtercollection/contains/)(Filter) | Restituisce true se l'elemento specificato è presente in questa collezione; altrimenti, false. |
| [CopyTo](../../aspose.tasks/filtercollection/copyto/)(Filter[], int) | Copia gli elementi di questa collezione nell'array specificato, a partire dall'indice dell'array specificato. |
| [GetEnumerator](../../aspose.tasks/filtercollection/getenumerator/)() | Restituisce un enumeratore per questa collezione. |
| [Remove](../../aspose.tasks/filtercollection/remove/)(Filter) | Rimuove la prima occorrenza di un oggetto specifico da questa collezione. |
| [ToList](../../aspose.tasks/filtercollection/tolist/)() | Converte una collezione di filtri in un elenco di oggetti [`Filter`](../filter/). |

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

* class [Filter](../filter/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


