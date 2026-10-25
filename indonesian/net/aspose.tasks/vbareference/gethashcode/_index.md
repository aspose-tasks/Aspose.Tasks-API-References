---
title: "VbaReference.GetHashCode"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode VbaReference. Mengembalikan nilai kode hash untuk VbaReference ini"
type: docs
weight: 50
url: /id/net/aspose.tasks/vbareference/gethashcode/
---
## VbaReference.GetHashCode method

Mengembalikan nilai kode hash untuk [`VbaReference`](../) ini.

```csharp
public override int GetHashCode()
```

### Nilai Kembali

Mengembalikan nilai kode hash untuk objek ini.

## Contoh

Menampilkan cara mendapatkan kode hash dari referensi VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

var reference1 = project.VbaProject.References.ToList()[0];
var reference2 = project.VbaProject.References.ToList()[1];

// Kode hash referensi adalah kode hash dari GUID referensi internal
Console.WriteLine("VBA reference Hash Code: {0}", reference1.GetHashCode());
Console.WriteLine("VBA reference Hash Code: {0}", reference2.GetHashCode());
```

### Lihat Juga

* class [VbaReference](../)
* namespace [Aspose.Tasks](../../vbareference/)
* assembly [Aspose.Tasks](../../../)


