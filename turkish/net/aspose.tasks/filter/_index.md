---
title: "Sınıf Filter"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Filter sınıfı. Proje içinde bir filtreyi temsil eder."
type: docs
weight: 600
url: /tr/net/aspose.tasks/filter/
---
## Filter class

Project içinde bir filtreyi temsil eder.

```csharp
public sealed class Filter : IComparable<Filter>, IEquatable<Filter>
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [Filter](filter/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Criteria](../../aspose.tasks/filter/criteria/) { get; set; } | Görevlerin veya kaynakların MSP görünümünde görüntülenmesi için karşılaması gereken ölçütü alır veya ayarlar. |
| [FilterType](../../aspose.tasks/filter/filtertype/) { get; set; } | Filtrenin türünü alır. |
| [Index](../../aspose.tasks/filter/index/) { get; } | `Filter` nesnesinin, Filters içeren nesnedeki dizinini alır. |
| [Name](../../aspose.tasks/filter/name/) { get; set; } | Bir Filter nesnesinin adını alır veya ayarlar. |
| [ShowInMenu](../../aspose.tasks/filter/showinmenu/) { get; set; } | Projenin, Ribbon'daki Görünüm sekmesindeki Filter açılır listesinde filtre adını gösterip göstermediğini belirten bir değeri alır veya ayarlar. |
| [ShowRelatedSummaryRows](../../aspose.tasks/filter/showrelatedsummaryrows/) { get; set; } | Filtre için ilişkili özet satırlarının görüntülenip görüntülenmeyeceğini belirten bir değeri alır veya ayarlar. |
| [Uid](../../aspose.tasks/filter/uid/) { get; } | Bir filtrenin benzersiz tanımlayıcısını alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [CompareTo](../../aspose.tasks/filter/compareto/)(Filter) | `Filter` sınıfının belirtilen örneğiyle bu örneği karşılaştırır ve bunların göreceli sırasını gösteren bir değer döndürür. |
| [Equals](../../aspose.tasks/filter/equals/#equals)(Filter) | Bu örneğin belirtilen AssignmentBaseline nesnesine eşit olup olmadığını gösteren bir değer döndürür. |
| override [Equals](../../aspose.tasks/filter/equals/#equals_1)(object) | Bu örneğin belirtilen AssignmentBaseline nesnesine eşit olup olmadığını gösteren bir değer döndürür. |
| override [GetHashCode](../../aspose.tasks/filter/gethashcode/)() | Filtre için bir karma kod değeri döndürür. |
| [operator ==](../../aspose.tasks/filter/op_equality/) | Bu örneğin belirtilen nesneye eşit olup olmadığını gösteren bir değer döndürür. |
| [operator &gt;](../../aspose.tasks/filter/op_greaterthan/) | Bu örneğin belirtilen nesneden büyük olup olmadığını gösteren bir değer döndürür. |
| [operator &gt;=](../../aspose.tasks/filter/op_greaterthanorequal/) | Bu örneğin belirtilen nesneden büyük veya ona eşit olup olmadığını gösteren bir değer döndürür. |
| [operator !=](../../aspose.tasks/filter/op_inequality/) | Bu örneğin belirtilen nesneye eşit olmadığını gösteren bir değer döndürür. |
| [operator &lt;](../../aspose.tasks/filter/op_lessthan/) | Bu örneğin belirtilen nesneden küçük olup olmadığını gösteren bir değer döndürür. |
| [operator &lt;=](../../aspose.tasks/filter/op_lessthanorequal/) | Bu örneğin belirtilen nesneden küçük veya ona eşit olup olmadığını gösteren bir değer döndürür. |

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


