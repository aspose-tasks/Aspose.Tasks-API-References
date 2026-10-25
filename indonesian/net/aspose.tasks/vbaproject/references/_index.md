---
title: "VbaProject.References"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti VbaProject. Mendapatkan koleksi VbaReferenceCollection"
type: docs
weight: 70
url: /id/net/aspose.tasks/vbaproject/references/
---
## VbaProject.References property

Mendapatkan koleksi [`VbaReferenceCollection`](../../vbareferencecollection/)

```csharp
public VbaReferenceCollection References { get; }
```

## Contoh

Menampilkan cara membaca informasi referensi proyek VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Reference count " + project.VbaProject.References.Count);

foreach (var reference in project.VbaProject.References)
{
    Console.WriteLine("Identifier: " + reference.LibIdentifier);
    Console.WriteLine("Name: " + reference.Name);
}
```

### Lihat Juga

* class [VbaReferenceCollection](../../vbareferencecollection/)
* class [VbaProject](../)
* namespace [Aspose.Tasks](../../vbaproject/)
* assembly [Aspose.Tasks](../../../)


