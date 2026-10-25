---
title: "Filter.ShowInMenu"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Filter özelliği. Projenin Şerit'in Görünüm sekmesindeki Filtre açılır listesinde filtre adını gösterip göstermeyeceğini belirten bir değeri alır veya ayarlar"
type: docs
weight: 60
url: /tr/net/aspose.tasks/filter/showinmenu/
---
## Filter.ShowInMenu property

Projenin, Ribbon'daki Görünüm sekmesindeki Filter açılır listesinde filtre adını gösterip göstermediğini belirten bir değeri alır veya ayarlar.

```csharp
public bool ShowInMenu { get; set; }
```

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

* class [Filter](../)
* namespace [Aspose.Tasks](../../filter/)
* assembly [Aspose.Tasks](../../../)


