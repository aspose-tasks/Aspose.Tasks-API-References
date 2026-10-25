---
title: "Prj.LastPrinted"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Prj field. Waktu cetak terakhir proyek. Disimpan dalam format UTC di file mpp. Tipe DateTime"
type: docs
weight: 430
url: /id/net/aspose.tasks/prj/lastprinted/
---
## Prj.LastPrinted field

Waktu cetak terakhir proyek. Disimpan dalam format UTC di file mpp. Tipe DateTime.

```csharp
public static readonly Key<DateTime, PrjKey> LastPrinted;
```

## Contoh

Menampilkan cara membaca/menulis properti Prj.LastPrinted.

```csharp
var project = new Project();

project.Set(Prj.LastPrinted, new DateTime(2020, 4, 10, 13, 0, 0));

Console.WriteLine("Last Printed: " + project.Get(Prj.LastPrinted));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


