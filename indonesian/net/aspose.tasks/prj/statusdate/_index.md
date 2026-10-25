---
title: "Prj.StatusDate"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Prj. tanggal status untuk menampilkan kemajuan atau menghitung total nilai yang diperoleh. Tanggal status sama dengan tanggal hari ini kecuali tanggal status yang berbeda ditentukan"
type: docs
weight: 690
url: /id/net/aspose.tasks/prj/statusdate/
---
## Prj.StatusDate field

tanggal status untuk menampilkan kemajuan atau menghitung total nilai yang diperoleh. Tanggal status sama dengan tanggal saat ini (tanggal hari ini) kecuali tanggal status yang berbeda ditentukan.

```csharp
public static readonly Key<DateTime, PrjKey> StatusDate;
```

## Contoh

Menampilkan cara membaca/menulis properti Prj.StatusDate.

```csharp
var project = new Project();

project.Set(Prj.StatusDate, new DateTime(2020, 4, 19, 8, 0, 0));

Console.WriteLine("Status Date: " + project.Get(Prj.StatusDate));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


