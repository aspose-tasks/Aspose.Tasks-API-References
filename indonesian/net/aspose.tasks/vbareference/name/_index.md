---
title: "VbaReference.Name"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti VbaReference. Mendapatkan atau mengatur nama referensi VBA"
type: docs
weight: 30
url: /id/net/aspose.tasks/vbareference/name/
---
## VbaReference.Name property

Mendapatkan atau mengatur nama referensi VBA.

```csharp
public string Name { get; set; }
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


