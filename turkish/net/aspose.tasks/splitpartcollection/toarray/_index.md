---
title: "SplitPartCollection.ToArray"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "SplitPartCollection yöntemi. Koleksiyondaki tüm parçaları yeni bir diziye kopyalar"
type: docs
weight: 40
url: /tr/net/aspose.tasks/splitpartcollection/toarray/
---
## SplitPartCollection.ToArray method

Koleksiyondaki tüm parçaları yeni bir diziye kopyalar.

```csharp
public SplitPart[] ToArray()
```

### Dönüş Değeri

[`SplitPart`](../../splitpart/) nesnelerinden oluşan bir dizi.

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

* class [SplitPart](../../splitpart/)
* class [SplitPartCollection](../)
* namespace [Aspose.Tasks](../../splitpartcollection/)
* assembly [Aspose.Tasks](../../../)


