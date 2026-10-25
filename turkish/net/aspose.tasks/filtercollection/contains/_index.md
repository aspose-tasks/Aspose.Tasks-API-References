---
title: "FilterCollection.Contains"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "FilterCollection yöntemi. Belirtilen öğe bu koleksiyonda bulunursa true, aksi takdirde false döndürür"
type: docs
weight: 50
url: /tr/net/aspose.tasks/filtercollection/contains/
---
## FilterCollection.Contains method

Belirtilen öğe bu koleksiyonda bulunursa true, aksi takdirde false döndürür.

```csharp
public bool Contains(Filter item)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| öğe | Filter | bulunacak belirtilen öğe. |

### Dönüş Değeri

Belirtilen öğe bu koleksiyonda bulunursa doğru; aksi takdirde yanlış.

## Örnekler

Filtre koleksiyonlarıyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "ReadFilterDefinitionData.mpp");

// görev filtreleri üzerinde yinele
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

// kaynak filtreleri üzerinde yinele
Console.WriteLine("Project.ResourceFilters count: " + project.ResourceFilters.Count);
foreach (var filter in project.ResourceFilters)
{
    Console.WriteLine("Resource Filter Item Type: Item.ResourceType: " + filter.FilterType);
    Console.WriteLine("Resource filter ShowInMenu" + filter.ShowInMenu);
    Console.WriteLine("Resource filter ShowRelatedSummaryRows: " + filter.ShowRelatedSummaryRows);
}

var otherProject = new Project(DataDir + "Blank2010.mpp");

// diğer projenin filtrelerini temizle
otherProject.TaskFilters.Clear();

// filtreleri diğer projeye kopyala
var filters = new Filter[project.TaskFilters.Count];
project.TaskFilters.CopyTo(filters, 0);

foreach (var filter in filters)
{
    otherProject.TaskFilters.Add(filter);
}

// özel görev filtresi ekle
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

// tüm filtreleri kaldır
List<Filter> filtersToDelete = otherProject.TaskFilters.ToList();
foreach (var filter in filtersToDelete)
{
    otherProject.TaskFilters.Remove(filter);
}
```

### Ayrıca Bakınız

* class [Filter](../../filter/)
* class [FilterCollection](../)
* namespace [Aspose.Tasks](../../filtercollection/)
* assembly [Aspose.Tasks](../../../)


