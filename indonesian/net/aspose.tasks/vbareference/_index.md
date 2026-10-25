---
title: "Kelas VbaReference"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.VbaReference. Mewakili referensi dari VbaProject."
type: docs
weight: 2870
url: /id/net/aspose.tasks/vbareference/
---
## VbaReference class

Mewakili referensi dari [`VbaProject`](../vbaproject/).

```csharp
public sealed class VbaReference : IEquatable<VbaReference>
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [VbaReference](vbareference/)() | Konstruktor default. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [LibIdentifier](../../aspose.tasks/vbareference/libidentifier/) { get; } | Mendapatkan pengidentifikasi pustaka. |
| [Name](../../aspose.tasks/vbareference/name/) { get; set; } | Mendapatkan atau mengatur nama referensi VBA. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| override [Equals](../../aspose.tasks/vbareference/equals/#equals_1)(object) | Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek `VbaReference` yang ditentukan. |
| [Equals](../../aspose.tasks/vbareference/equals/#equals)(VbaReference) | Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek `VbaReference` yang ditentukan. |
| override [GetHashCode](../../aspose.tasks/vbareference/gethashcode/)() | Mengembalikan nilai kode hash untuk `VbaReference` ini. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


