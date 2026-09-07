---
title: "Prj.CurrentDate"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Prj field. Tanggal sistem"
type: docs
weight: 190
url: /id/net/aspose.tasks/prj/currentdate/
---
## Prj.CurrentDate field

Tanggal sistem.

```csharp
public static readonly Key<DateTime, PrjKey> CurrentDate;
```

## Contoh

Menampilkan cara membaca/menulis properti Prj.CurrentDate.

```csharp
var project = new Project();

project.Set(Prj.CurrentDate, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Current Date: " + project.Get(Prj.CurrentDate));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


