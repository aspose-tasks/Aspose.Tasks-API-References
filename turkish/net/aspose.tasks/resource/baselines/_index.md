---
title: "Resource.Baselines"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Resource özelliği. Bu nesne için bir BaselineCollection örneği alır. Bir kaynak için temel değerler"
type: docs
weight: 160
url: /tr/net/aspose.tasks/resource/baselines/
---
## Resource.Baselines property

Bu nesne için bir BaselineCollection örneğini alır. Bir kaynak için temel değerler.

```csharp
public BaselineCollection Baselines { get; }
```

## Örnekler

Kaynağın temel değerlerini nasıl okuyacağınızı gösterir.

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

foreach (var resource in project.Resources)
{
    foreach (var baseline in resource.Baselines)
    {
        Console.WriteLine("BaselineNumber: " + baseline.BaselineNumber);
        Console.WriteLine("Bcwp: " + baseline.Bcwp);
        Console.WriteLine("Bcws: " + baseline.Bcws);
        Console.WriteLine("Cost: " + baseline.Cost);
        Console.WriteLine("Work: " + baseline.Work);
    }
}
```

### Ayrıca Bakınız

* class [BaselineCollection](../../baselinecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


