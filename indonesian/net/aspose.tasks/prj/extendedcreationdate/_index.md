---
title: "Prj.ExtendedCreationDate"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Prj field. Tanggal yang digunakan untuk perhitungan dan pelaporan"
type: docs
weight: 320
url: /id/net/aspose.tasks/prj/extendedcreationdate/
---
## Prj.ExtendedCreationDate field

Tanggal yang digunakan untuk perhitungan dan pelaporan.

```csharp
public static readonly Key<DateTime, PrjKey> ExtendedCreationDate;
```

## Contoh

Menampilkan cara membaca/menulis properti Prj.ExtendedCreationDate.

```csharp
var project = new Project();

project.Set(Prj.ExtendedCreationDate, new DateTime(2020, 4, 10, 9, 0, 0));

Console.WriteLine("Extended Creation Date: " + project.Get(Prj.ExtendedCreationDate));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


