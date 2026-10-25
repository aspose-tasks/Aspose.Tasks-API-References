---
title: "Enum ItemType"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.ItemType enum. Bir öğenin türünü belirtir"
type: docs
weight: 920
url: /tr/net/aspose.tasks/itemtype/
---
## ItemType enumeration

Bir öğenin türünü belirtir.

```csharp
public enum ItemType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| TaskItem | `0` | Görev öğesi. |
| ResourceItem | `1` | Kaynak öğesi. |
| OtherItem | `2` | Diğer öğe. |

## Örnekler

Filtrelerle nasıl çalışılacağını gösterir.

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

// kaynak filtrelerini kontrol et
List<Filter> resourceFilters = project.ResourceFilters.ToList();
Console.WriteLine("Project.ResourceFilters count: " + resourceFilters.Count);
Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + resourceFilters[0].FilterType);
Console.WriteLine("Resource filter ShowInMenu" + resourceFilters[0].ShowInMenu);
Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + resourceFilters[0].ShowRelatedSummaryRows);
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


