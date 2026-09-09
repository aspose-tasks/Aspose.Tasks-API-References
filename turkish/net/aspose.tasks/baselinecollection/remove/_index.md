---
title: "BaselineCollection.Remove"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "BaselineCollection yöntemi. Bu koleksiyondan baseline'ı kaldırır"
type: docs
weight: 60
url: /tr/net/aspose.tasks/baselinecollection/remove/
---
## BaselineCollection.Remove method

Bu koleksiyondan temel çizgiyi kaldırır.

```csharp
public bool Remove(Baseline item)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| öğe | Baseline | Kaldırılacak öğe. |

### Dönüş Değeri

[`Baseline`](../../baseline/) örneği başarıyla kaldırıldıysa true; aksi takdirde false

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

* class [Baseline](../../baseline/)
* class [BaselineCollection](../)
* namespace [Aspose.Tasks](../../baselinecollection/)
* assembly [Aspose.Tasks](../../../)


