---
title: "VbaProject.References"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "VbaProject özelliği. VbaReferenceCollection koleksiyonunu alır"
type: docs
weight: 70
url: /tr/net/aspose.tasks/vbaproject/references/
---
## VbaProject.References property

[`VbaReferenceCollection`](../../vbareferencecollection/) koleksiyonunu alır

```csharp
public VbaReferenceCollection References { get; }
```

## Örnekler

VBA proje referans bilgilerini nasıl okuyacağınızı gösterir.

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

* class [VbaReferenceCollection](../../vbareferencecollection/)
* class [VbaProject](../)
* namespace [Aspose.Tasks](../../vbaproject/)
* assembly [Aspose.Tasks](../../../)


