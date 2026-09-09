---
title: "Sınıf VbaModuleAttributeCollection"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.VbaModuleAttributeCollection sınıfı. VbaModuleAttribute nesnelerinin bir koleksiyonunu temsil eder."
type: docs
weight: 2830
url: /tr/net/aspose.tasks/vbamoduleattributecollection/
---
## VbaModuleAttributeCollection class

[`VbaModuleAttribute`](../vbamoduleattribute/) nesnelerinin bir koleksiyonunu temsil eder.

```csharp
public class VbaModuleAttributeCollection : ReadOnlyCollectionBase<VbaModuleAttribute>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../aspose.tasks/readonlycollectionbase-1/count/) { get; } |  |
| [Item](../../aspose.tasks/readonlycollectionbase-1/item/) { get; set; } |  |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.tasks/readonlycollectionbase-1/add/)(VbaModuleAttribute) |  |
| [GetEnumerator](../../aspose.tasks/readonlycollectionbase-1/getenumerator/)() |  |
| [ToList](../../aspose.tasks/readonlycollectionbase-1/tolist/)() |  |

## Örnekler

VBA modülünün öznitelik koleksiyonunda nasıl yineleme yapılacağını gösterir.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Attributes Count: " + module.Attributes.Count);
    foreach (var attribute in module.Attributes)
    {
        Console.WriteLine("Attribute Name: " + attribute.Key);
        Console.WriteLine("Attribute Value: " + attribute.Value);
    }
}
```

### Ayrıca Bakınız

* class [ReadOnlyCollectionBase&lt;T&gt;](../readonlycollectionbase-1/)
* class [VbaModuleAttribute](../vbamoduleattribute/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


