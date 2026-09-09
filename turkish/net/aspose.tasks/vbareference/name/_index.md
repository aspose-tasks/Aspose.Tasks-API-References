---
title: "VbaReference.Name"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "VbaReference özelliği. VBA referansının adını alır veya ayarlar"
type: docs
weight: 30
url: /tr/net/aspose.tasks/vbareference/name/
---
## VbaReference.Name property

VBA referansının adını alır veya ayarlar.

```csharp
public string Name { get; set; }
```

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

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)


