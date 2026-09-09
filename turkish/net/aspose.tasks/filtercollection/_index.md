---
title: "Sınıf FilterCollection"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.FilterCollection sınıfı. Filter nesnelerinin bir listesini içerir. ICollectionFilter arayüzünü uygular"
type: docs
weight: 610
url: /tr/net/aspose.tasks/filtercollection/
---
## FilterCollection class

`[`Filter`](../filter/)` nesnelerinin bir listesini içerir. ICollection&lt;Filter&gt; arayüzünü uygular.

```csharp
public class FilterCollection : ICollection<Filter>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../aspose.tasks/filtercollection/count/) { get; } | Bu koleksiyonda bulunan öğe sayısını alır. |
| [IsReadOnly](../../aspose.tasks/filtercollection/isreadonly/) { get; } | Bu koleksiyonun yalnızca okunur olup olmadığını gösteren bir değer alır; aksi takdirde false. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.tasks/filtercollection/add/)(Filter) | Belirtilen öğeyi bu koleksiyona ekler. |
| [Clear](../../aspose.tasks/filtercollection/clear/)() | Bu koleksiyondaki tüm öğeleri kaldırır. |
| [Contains](../../aspose.tasks/filtercollection/contains/)(Filter) | Belirtilen öğe bu koleksiyonda bulunursa true, aksi takdirde false döndürür. |
| [CopyTo](../../aspose.tasks/filtercollection/copyto/)(Filter[], int) | Bu koleksiyonun öğelerini belirtilen diziye, belirtilen dizi indeksinden başlayarak kopyalar. |
| [GetEnumerator](../../aspose.tasks/filtercollection/getenumerator/)() | Bu koleksiyon için bir enumerator döndürür. |
| [Remove](../../aspose.tasks/filtercollection/remove/)(Filter) | Bu koleksiyondan belirli bir nesnenin ilk oluşumunu kaldırır. |
| [ToList](../../aspose.tasks/filtercollection/tolist/)() | Bir filtre koleksiyonunu [`Filter`](../filter/) nesnelerinin listesine dönüştürür. |

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

* class [Filter](../filter/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


