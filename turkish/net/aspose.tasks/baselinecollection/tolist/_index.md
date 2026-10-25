---
title: "BaselineCollection.ToList"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "BaselineCollection yöntemi. BaselineCollection nesnesini Baseline nesnelerinden oluşan bir listeye dönüştürür"
type: docs
weight: 70
url: /tr/net/aspose.tasks/baselinecollection/tolist/
---
## BaselineCollection.ToList method

BaselineCollection nesnesini [`Baseline`](../../baseline/) nesnelerinden oluşan bir listeye dönüştürür.

```csharp
public List<Baseline> ToList()
```

### Dönüş Değeri

[`Baseline`](../../baseline/) nesnelerinden oluşan bir liste.

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


