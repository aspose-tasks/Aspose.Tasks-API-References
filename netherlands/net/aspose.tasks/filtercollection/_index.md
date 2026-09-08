---
title: "Klasse FilterCollection"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.FilterCollection klasse. Bevat een lijst met Filter-objecten. Implementeert de ICollectionFilter-interface."
type: docs
weight: 610
url: /nl/net/aspose.tasks/filtercollection/
---
## FilterCollection class

Bevat een lijst met [`Filter`](../filter/) objecten. Implementeert de ICollection&lt;Filter&gt;-interface.

```csharp
public class FilterCollection : ICollection<Filter>
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Count](../../aspose.tasks/filtercollection/count/) { get; } | Haalt het aantal elementen op dat in deze collectie zit. |
| [IsReadOnly](../../aspose.tasks/filtercollection/isreadonly/) { get; } | Haalt een waarde op die aangeeft of deze collectie alleen-lezen is; anders, false. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Add](../../aspose.tasks/filtercollection/add/)(Filter) | Voegt het opgegeven item toe aan deze collectie. |
| [Clear](../../aspose.tasks/filtercollection/clear/)() | Verwijdert alle items uit deze collectie. |
| [Contains](../../aspose.tasks/filtercollection/contains/)(Filter) | Retourneert true als het opgegeven item in deze collectie wordt gevonden; anders false. |
| [CopyTo](../../aspose.tasks/filtercollection/copyto/)(Filter[], int) | Kopieert de elementen van deze collectie naar de opgegeven array, beginnend bij de opgegeven array-index. |
| [GetEnumerator](../../aspose.tasks/filtercollection/getenumerator/)() | Retourneert een enumerator voor deze collectie. |
| [Remove](../../aspose.tasks/filtercollection/remove/)(Filter) | Verwijdert de eerste instantie van een specifiek object uit deze collectie. |
| [ToList](../../aspose.tasks/filtercollection/tolist/)() | Converteert een filtercollectie naar een lijst met [`Filter`](../filter/) objecten. |

## Voorbeelden

Toont hoe u met filtercollecties werkt.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");

// itereren over taakfilters
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

// itereren over resourcefilters
Console.WriteLine("Project.ResourceFilters count: " + project.ResourceFilters.Count);
foreach (var filter in project.ResourceFilters)
{
    Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + filter.FilterType);
    Console.WriteLine("Resource filter ShowInMenu" + filter.ShowInMenu);
    Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + filter.ShowRelatedSummaryRows);
}

var otherProject = new Project(DataDir + "Blank2010.mpp");

// wis de filters van een ander project
otherProject.TaskFilters.Clear();

// kopieer filters naar een ander project
var filters = new Filter[project.TaskFilters.Count];
project.TaskFilters.CopyTo(filters, 0);

foreach (var filter in filters)
{
    otherProject.TaskFilters.Add(filter);
}

// voeg een aangepaste taakfilter toe
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

// verwijder alle filters
List<Filter> filtersToDelete = otherProject.TaskFilters.ToList();
foreach (var filter in filtersToDelete)
{
    otherProject.TaskFilters.Remove(filter);
}
```

### Zie ook

* class [Filter](../filter/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


