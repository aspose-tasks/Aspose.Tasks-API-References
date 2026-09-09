---
title: "VbaModuleCollection.ToList"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "VbaModuleCollection yöntemi. Koleksiyon nesnesini VbaModule nesnelerinin bir listesine dönüştürür."
type: docs
weight: 100
url: /tr/net/aspose.tasks/vbamodulecollection/tolist/
---
## VbaModuleCollection.ToList method

Koleksiyon nesnesini [`VbaModule`](../../vbamodule/) nesnelerinin bir listesine dönüştürür.

```csharp
public List<VbaModule> ToList()
```

### Dönüş Değeri

Nesnelerin listesi.

## Örnekler

VBA modülleri üzerinde nasıl yineleme yapılacağını gösterir.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
var vbaProject = project.VbaProject;

Console.WriteLine("Total Modules Count: " + vbaProject.Modules.Count);
foreach (VbaModule module in vbaProject.Modules)
{
    Console.WriteLine("Module Name: " + module.Name);
    Console.WriteLine("Module Type: " + module.Type);
    Console.WriteLine("Source Code: " + module.SourceCode);
    Console.WriteLine();
}
```

### Ayrıca Bakınız

* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Tasks](../../vbamodulecollection/)
* assembly [Aspose.Tasks](../../../)


