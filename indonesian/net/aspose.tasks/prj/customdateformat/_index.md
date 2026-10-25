---
title: "Prj.CustomDateFormat"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Prj. Format tanggal khusus tampilan proyek. Digunakan untuk memformat tanggal ketika properti DateFormat diatur ke Custom"
type: docs
weight: 200
url: /id/net/aspose.tasks/prj/customdateformat/
---
## Prj.CustomDateFormat field

Format tanggal khusus tampilan proyek. Digunakan untuk memformat tanggal ketika properti [`DateFormat`](../dateformat/) diatur ke Custom.

```csharp
public static readonly Key<string, PrjKey> CustomDateFormat;
```

## Contoh

Menampilkan cara membaca/menulis properti Prj.CustomDateFormat.

```csharp
var project = new Project();

project.Set(Prj.CustomDateFormat, "dd MMMM yyyy H:mm");

Console.WriteLine("Custom Date Format: " + project.Get(Prj.CustomDateFormat));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


