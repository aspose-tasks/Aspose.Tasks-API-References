---
title: "Prj.CreationDate"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Prj. Tanggal dan waktu ketika sebuah proyek dibuat"
type: docs
weight: 130
url: /id/net/aspose.tasks/prj/creationdate/
---
## Prj.CreationDate field

Tanggal dan waktu saat proyek dibuat.

```csharp
public static readonly Key<DateTime, PrjKey> CreationDate;
```

## Catatan

Disimpan dalam format UTC di file mpp. Tipe DateTime.

## Contoh

Menampilkan cara membaca/menulis properti Prj.CreationDate.

```csharp
var project = new Project();

project.Set(Prj.CreationDate, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Creation Date: " + project.Get(Prj.CreationDate));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


