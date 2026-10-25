---
title: "Prj.TimescaleStart"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Prj. Tanggal ketika skala waktu dalam tampilan dimulai"
type: docs
weight: 740
url: /id/net/aspose.tasks/prj/timescalestart/
---
## Prj.TimescaleStart field

Tanggal ketika skala waktu dalam tampilan dimulai.

```csharp
public static readonly Key<DateTime, PrjKey> TimescaleStart;
```

## Contoh

Menampilkan cara mengatur tanggal mulai skala waktu untuk menyesuaikan tanggal di mana tampilan harus dimulai.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.TimescaleStart, new DateTime(2012, 4, 30));

Console.WriteLine("Timescale Start: " + project.Get(Prj.TimescaleStart));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


