---
title: "SplitPartCollection sınıfı"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.SplitPartCollection sınıfı. Bir görevin bölümlerini temsil eden koleksiyon."
type: docs
weight: 2300
url: /tr/net/aspose.tasks/splitpartcollection/
---
## SplitPartCollection class

Bir görevin bölümlerini temsil eden koleksiyon.

```csharp
public class SplitPartCollection : IList<SplitPart>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../aspose.tasks/splitpartcollection/count/) { get; } | Koleksiyondaki parça sayısını alır. |
| [Item](../../aspose.tasks/splitpartcollection/item/) { get; set; } | Belirtilen indeksteki görevin bölünmüş parçasını getirir. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [GetEnumerator](../../aspose.tasks/splitpartcollection/getenumerator/)() | Bu koleksiyon için bir enumerator döndürür. |
| [ToArray](../../aspose.tasks/splitpartcollection/toarray/)() | Koleksiyondaki tüm parçaları yeni bir diziye kopyalar. |

## Örnekler

Bölünmüş parça koleksiyonlarıyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "Splits.mpp");

var task = project.RootTask.Children.GetById(1);

// bölünmüş parçalar üzerinde yineleme yap
Console.WriteLine("Iterate over split parts");
Console.WriteLine("Split parts count:" + task.SplitParts.Count);
foreach (var splitPart in task.SplitParts)
{
    Console.WriteLine("Start: " + splitPart.Start);
    Console.WriteLine("Finish: " + splitPart.Finish);
}

// parçayı indeksle al
var split = task.SplitParts[0];
Console.WriteLine("Split start: " + split.Start);

// görevin ilk bölünmüş parçasıyla bazı işlemler yap
```

### Ayrıca Bakınız

* class [SplitPart](../splitpart/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


