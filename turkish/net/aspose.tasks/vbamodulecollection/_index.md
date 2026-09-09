---
title: "Sınıf VbaModuleCollection"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.VbaModuleCollection sınıfı. VbaModule nesnelerinin bir koleksiyonunu temsil eder"
type: docs
weight: 2840
url: /tr/net/aspose.tasks/vbamodulecollection/
---
## VbaModuleCollection class

[`VbaModule`](../vbamodule/) nesnelerinin bir koleksiyonunu temsil eder.

```csharp
public class VbaModuleCollection : ICollection<VbaModule>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../aspose.tasks/vbamodulecollection/count/) { get; } |  |
| [IsReadOnly](../../aspose.tasks/vbamodulecollection/isreadonly/) { get; } |  |
| [Item](../../aspose.tasks/vbamodulecollection/item/) { get; } | Belirtilen indeksteki modülü alır. (2 indeksleyici) |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.tasks/vbamodulecollection/add/)(VbaModule) |  |
| [Clear](../../aspose.tasks/vbamodulecollection/clear/)() |  |
| [Contains](../../aspose.tasks/vbamodulecollection/contains/)(VbaModule) |  |
| [CopyTo](../../aspose.tasks/vbamodulecollection/copyto/)(VbaModule[], int) |  |
| [GetEnumerator](../../aspose.tasks/vbamodulecollection/getenumerator/)() |  |
| [Remove](../../aspose.tasks/vbamodulecollection/remove/)(VbaModule) |  |
| [ToList](../../aspose.tasks/vbamodulecollection/tolist/)() | Koleksiyon nesnesini [`VbaModule`](../vbamodule/) nesnelerinin bir listesine dönüştürür. |

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

* class [VbaModule](../vbamodule/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


