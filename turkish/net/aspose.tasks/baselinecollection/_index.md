---
title: "Sınıf BaselineCollection"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.BaselineCollection sınıfı. Baseline nesnelerinin bir koleksiyonunu temsil eder"
type: docs
weight: 120
url: /tr/net/aspose.tasks/baselinecollection/
---
## BaselineCollection class

[`Baseline`](../baseline/) nesnelerinin bir koleksiyonunu temsil eder.

```csharp
public class BaselineCollection : IList<Baseline>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../aspose.tasks/baselinecollection/count/) { get; } | Bu BaselineCollection nesnesinde bulunan nesne sayısını alır. |
| [Item](../../aspose.tasks/baselinecollection/item/) { get; set; } | Belirtilen indeksteki öğeyi döndürür. |
| [ParentResource](../../aspose.tasks/baselinecollection/parentresource/) { get; } | Bu koleksiyon için üst [`Resource`](../resource/) öğesini alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.tasks/baselinecollection/add/)(Baseline) | Bu, ICollection'ın Add metodunun sadece NotSupportedException fırlatan taslak uygulamasıdır |
| [GetEnumerator](../../aspose.tasks/baselinecollection/getenumerator/)() | Bu koleksiyon için bir enumerator döndürür. |
| [Remove](../../aspose.tasks/baselinecollection/remove/)(Baseline) | Bu koleksiyondan temel çizgiyi kaldırır. |
| [ToList](../../aspose.tasks/baselinecollection/tolist/)() | BaselineCollection nesnesini [`Baseline`](../baseline/) nesnelerinin listesine dönüştürür. |

## Örnekler

Baseline koleksiyonlarıyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "WorkWithBaselineCollection.mpp");
var resource = project.Resources.GetByUid(1);

Console.WriteLine("Count of assignment baselines: " + resource.Baselines.Count);
Console.WriteLine("Parent Resource Name: " + resource.Baselines.ParentResource.Get(Rsc.Name));

// baseline bilgilerini oku
foreach (var baseline in resource.Baselines)
{
    Console.WriteLine("Baseline Number: " + baseline.BaselineNumber);
    Console.WriteLine("Cost: " + baseline.Cost);
    Console.WriteLine("Work: " + baseline.Work);
    Console.WriteLine("BCWP: " + baseline.Bcwp);
    Console.WriteLine("BCWS: " + baseline.Bcws);
    Console.WriteLine();
}

Console.WriteLine("Delete all baselines: ");
List<Baseline> baselines = resource.Baselines.ToList();
foreach (var baseline in baselines)
{
    Console.WriteLine("Delete baseline with name: " + baseline.BaselineNumber);
    resource.Baselines.Remove(baseline);
}
```

### Ayrıca Bakınız

* class [Baseline](../baseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


