---
title: "FilterCollection.CopyTo"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "FilterCollection-methode. Kopieert de elementen van deze collectie naar de opgegeven array, beginnend bij de opgegeven array-index"
type: docs
weight: 60
url: /nl/net/aspose.tasks/filtercollection/copyto/
---
## FilterCollection.CopyTo method

Kopieert de elementen van deze collectie naar de opgegeven array, beginnend bij de opgegeven array-index.

```csharp
public void CopyTo(Filter[] array, int arrayIndex)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| array | Filter[] | de opgegeven eendimensionale array om elementen naartoe te kopiëren |
| arrayIndex | Int32 | de nulgebaseerde index van de opgegeven array waarop het kopiëren begint. |

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

* class [Filter](../../filter/)
* class [FilterCollection](../)
* namespace [Aspose.Tasks](../../filtercollection/)
* assembly [Aspose.Tasks](../../../)


