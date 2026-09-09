---
title: "Class VbaModuleAttribute"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.VbaModuleAttribute sınıfı. VbaModule nesnesinin özelliği"
type: docs
weight: 2820
url: /tr/net/aspose.tasks/vbamoduleattribute/
---
## VbaModuleAttribute class

[`VbaModule`](../vbamodule/) nesnesinin özelliği

```csharp
public sealed class VbaModuleAttribute : IEquatable<VbaModuleAttribute>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Key](../../aspose.tasks/vbamoduleattribute/key/) { get; } | VBA modül özelliğinin anahtarını alır. |
| [Value](../../aspose.tasks/vbamoduleattribute/value/) { get; } | VBA modül özelliğinin değerini alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [Equals](../../aspose.tasks/vbamoduleattribute/equals/#equals_1)(object) | Belirtilen `VbaModuleAttribute` nesnesine eşit olup olmadığını gösteren bir değer döndürür. |
| [Equals](../../aspose.tasks/vbamoduleattribute/equals/#equals)(VbaModuleAttribute) | Belirtilen `VbaModuleAttribute` nesnesine eşit olup olmadığını gösteren bir değer döndürür. |
| override [GetHashCode](../../aspose.tasks/vbamoduleattribute/gethashcode/)() | Bu `VbaModuleAttribute` için bir karma kod değeri döndürür. |

## Örnekler

VBA modül öznitelikleriyle nasıl çalışılacağını gösterir.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Attributes Count: " + module.Attributes.Count);
    foreach (var attribute in module.Attributes)
    {
        Console.WriteLine("  VB Name: " + attribute.Key);
        Console.WriteLine("  Module: " + attribute.Value);
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


