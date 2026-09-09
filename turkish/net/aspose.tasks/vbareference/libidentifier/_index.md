---
title: "VbaReference.LibIdentifier"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "VbaReference özelliği. Kitaplığın tanımlayıcısını alır"
type: docs
weight: 20
url: /tr/net/aspose.tasks/vbareference/libidentifier/
---
## VbaReference.LibIdentifier property

Kütüphanenin tanımlayıcısını alır.

```csharp
public string LibIdentifier { get; }
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


