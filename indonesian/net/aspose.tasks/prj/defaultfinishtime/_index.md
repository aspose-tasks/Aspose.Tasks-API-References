---
title: "Prj.DefaultFinishTime"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Prj field. Waktu selesai default untuk tugas baru"
type: docs
weight: 230
url: /id/net/aspose.tasks/prj/defaultfinishtime/
---
## Prj.DefaultFinishTime field

Waktu selesai default untuk tugas baru.

```csharp
public static readonly Key<DateTime, PrjKey> DefaultFinishTime;
```

## Contoh

Menampilkan cara membaca/menulis properti Prj.DefaultFinishTime.

```csharp
var project = new Project();

project.Set(Prj.DefaultFinishTime, new DateTime(2000, 1, 3, 10, 0, 0));

Console.WriteLine("Default Finish Time: " + project.Get(Prj.DefaultFinishTime));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


