---
title: "Filter.FilterType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Filter. Λαμβάνει τον τύπο του φίλτρου."
type: docs
weight: 30
url: /el/net/aspose.tasks/filter/filtertype/
---
## Filter.FilterType property

Λαμβάνει τον τύπο του φίλτρου.

```csharp
public ItemType FilterType { get; set; }
```

## Παραδείγματα

Δείχνει πώς να εργαστείτε με φίλτρα.

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

// ελέγξτε τα φίλτρα πόρων
List<Filter> resourceFilters = project.ResourceFilters.ToList();
Console.WriteLine("Project.ResourceFilters count: " + resourceFilters.Count);
Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + resourceFilters[0].FilterType);
Console.WriteLine("Resource filter ShowInMenu" + resourceFilters[0].ShowInMenu);
Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + resourceFilters[0].ShowRelatedSummaryRows);
```

### Δείτε επίσης

* enum [ItemType](../../itemtype/)
* class [Filter](../)
* namespace [Aspose.Tasks](../../filter/)
* assembly [Aspose.Tasks](../../../)


