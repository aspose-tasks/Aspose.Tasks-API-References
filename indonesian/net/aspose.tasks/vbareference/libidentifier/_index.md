---
title: "VbaReference.LibIdentifier"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "VbaReference properti. Mendapatkan pengidentifikasi perpustakaan"
type: docs
weight: 20
url: /id/net/aspose.tasks/vbareference/libidentifier/
---
## VbaReference.LibIdentifier property

Mendapatkan pengidentifikasi pustaka.

```csharp
public string LibIdentifier { get; }
```

## Contoh

Menampilkan cara membaca referensi VBA.

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

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)


