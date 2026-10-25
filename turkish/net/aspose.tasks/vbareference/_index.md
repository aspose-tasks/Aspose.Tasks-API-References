---
title: "VbaReference sınıfı"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.VbaReference sınıfı. VbaProject'in bir referansını temsil eder."
type: docs
weight: 2870
url: /tr/net/aspose.tasks/vbareference/
---
## VbaReference class

[`VbaProject`](../vbaproject/) referansını temsil eder.

```csharp
public sealed class VbaReference : IEquatable<VbaReference>
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [VbaReference](vbareference/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [LibIdentifier](../../aspose.tasks/vbareference/libidentifier/) { get; } | Kütüphanenin tanımlayıcısını alır. |
| [Name](../../aspose.tasks/vbareference/name/) { get; set; } | VBA referansının adını alır veya ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| override [Equals](../../aspose.tasks/vbareference/equals/#equals_1)(object) | `VbaReference` nesnesine eşit olup olmadığını gösteren bir değer döndürür. |
| [Equals](../../aspose.tasks/vbareference/equals/#equals)(VbaReference) | `VbaReference` nesnesine eşit olup olmadığını gösteren bir değer döndürür. |
| override [GetHashCode](../../aspose.tasks/vbareference/gethashcode/)() | Bu `VbaReference` için bir karma kod değeri döndürür. |

## Örnekler

VBA referanslarını okumanın nasıl yapılacağını gösterir.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Reference count " + project.VbaProject.References.Count);

foreach (var reference in project.VbaProject.References)
{
    Console.WriteLine("Identifier: " + reference.LibIdentifier);
    Console.WriteLine("Name: " + reference.Name);
}
```

### Ayrıca Bakınız

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


