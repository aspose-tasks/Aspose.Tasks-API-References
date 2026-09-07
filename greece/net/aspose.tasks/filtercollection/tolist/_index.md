---
title: "FilterCollection.ToList"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "FilterCollection μέθοδος. Μετατρέπει μια συλλογή φίλτρων σε λίστα αντικειμένων Filter"
type: docs
weight: 90
url: /el/net/aspose.tasks/filtercollection/tolist/
---
## FilterCollection.ToList method

Μετατρέπει μια συλλογή φίλτρων σε λίστα αντικειμένων [`Filter`](../../filter/).

```csharp
public List<Filter> ToList()
```

### Τιμή Επιστροφής

Γενική λίστα αντικειμένων [`Filter`](../../filter/).

## Παραδείγματα

Δείχνει πώς να εργαστείτε με συλλογές φίλτρων.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");

// Επανάληψη στα φίλτρα εργασιών.
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

// Επανάληψη στα φίλτρα πόρων.
Console.WriteLine("Project.ResourceFilters count: " + project.ResourceFilters.Count);
foreach (var filter in project.ResourceFilters)
{
    Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + filter.FilterType);
    Console.WriteLine("Resource filter ShowInMenu" + filter.ShowInMenu);
    Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + filter.ShowRelatedSummaryRows);
}

var otherProject = new Project(DataDir + "Blank2010.mpp");

// Καθαρίστε τα φίλτρα του άλλου έργου.
otherProject.TaskFilters.Clear();

// Αντιγράψτε τα φίλτρα σε άλλο έργο.
var filters = new Filter[project.TaskFilters.Count];
project.TaskFilters.CopyTo(filters, 0);

foreach (var filter in filters)
{
    otherProject.TaskFilters.Add(filter);
}

// Προσθέστε προσαρμοσμένο φίλτρο εργασίας.
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

// Αφαιρέστε όλα τα φίλτρα.
List<Filter> filtersToDelete = otherProject.TaskFilters.ToList();
foreach (var filter in filtersToDelete)
{
    otherProject.TaskFilters.Remove(filter);
}
```

### Δείτε επίσης

* class [Filter](../../filter/)
* class [FilterCollection](../)
* namespace [Aspose.Tasks](../../filtercollection/)
* assembly [Aspose.Tasks](../../../)


