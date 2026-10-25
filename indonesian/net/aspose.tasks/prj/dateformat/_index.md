---
title: "Prj.DateFormat"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Prj. Format tanggal tampilan proyek"
type: docs
weight: 210
url: /id/net/aspose.tasks/prj/dateformat/
---
## Prj.DateFormat field

Format tanggal tampilan proyek.

```csharp
public static readonly Key<DateFormat, PrjKey> DateFormat;
```

## Contoh

Menampilkan cara membaca/menulis properti Prj.DateFormat.

```csharp
var project = new Project();

project.Set(Prj.DateFormat, DateFormat.DateDd);

Console.WriteLine("Date Format: " + project.Get(Prj.DateFormat));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [DateFormat](../../dateformat/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


