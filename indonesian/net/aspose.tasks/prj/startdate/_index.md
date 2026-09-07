---
title: "Prj.StartDate"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Prj. Tanggal mulai sebuah proyek"
type: docs
weight: 680
url: /id/net/aspose.tasks/prj/startdate/
---
## Prj.StartDate field

Tanggal mulai proyek.

```csharp
public static readonly Key<DateTime, PrjKey> StartDate;
```

## Contoh

Menunjukkan cara membaca/menulis properti Prj.StartDate.

```csharp
var project = new Project();

project.Set(Prj.StartDate, new DateTime(2020, 4, 19, 8, 0, 0));

Console.WriteLine("Start Date: " + project.Get(Prj.StartDate));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


