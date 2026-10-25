---
title: "SplitPartCollection.Item"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "SplitPartCollection özelliği. Belirtilen dizinde bir görev bölünmüş parçasını alır"
type: docs
weight: 20
url: /tr/net/aspose.tasks/splitpartcollection/item/
---
## SplitPartCollection indexer

Belirtilen indeksteki görevin bölünmüş parçasını getirir.

```csharp
public SplitPart this[int index] { get; set; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | Parça indeksi. |

### Dönüş Değeri

bir bölünmüş parça.

## Açıklamalar

Dizin sıfır tabanlıdır. Dizin dizi sınırlarının dışındaysa null döndürür.

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


