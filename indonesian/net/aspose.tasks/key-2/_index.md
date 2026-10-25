---
title: "Struktur KeyTK"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.Key2TK struct. Mewakili kunci properti dari kelas dengan tipe yang ditentukan. Sebuah instance dari kelas ini digunakan saat mendapatkan atau mengatur properti dari sebuah kontainer"
type: docs
weight: 930
url: /id/net/aspose.tasks/key-2/
---
## Key&lt;T,K&gt; structure

Mewakili kunci properti dari sebuah kelas dengan tipe yang ditentukan. Sebuah instance dari kelas ini digunakan saat mengambil atau mengatur properti dari sebuah kontainer.

```csharp
public struct Key<T, K>
    where K : struct
```

| Parameter | Deskripsi |
| --- | --- |
| T | Tipe nilai properti. |
| K | Tipe kunci properti. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [KeyType](../../aspose.tasks/key-2/keytype/) { get; } | Mendapatkan kunci properti. |

## Contoh

Menampilkan cara membaca/menulis properti Prj.ActualsInSync.

```csharp
var project = new Project();

project.Set(Prj.ActualsInSync, true);

Console.WriteLine("Actuals In Sync: " + project.Get(Prj.ActualsInSync));
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


