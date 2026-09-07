---
title: "Απαρίθμηση ItemType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.ItemType απαρίθμηση. Καθορίζει τον τύπο ενός αντικειμένου."
type: docs
weight: 920
url: /el/net/aspose.tasks/itemtype/
---
## ItemType enumeration

Καθορίζει τον τύπο ενός αντικειμένου.

```csharp
public enum ItemType
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| TaskItem | `0` | Αντικείμενο εργασίας. |
| ResourceItem | `1` | Αντικείμενο πόρου. |
| OtherItem | `2` | Άλλο αντικείμενο. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


