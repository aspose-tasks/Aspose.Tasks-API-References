---
title: "Prj.TimescaleFinish"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Prj. Tanggal ketika skala waktu dalam tampilan selesai"
type: docs
weight: 730
url: /id/net/aspose.tasks/prj/timescalefinish/
---
## Prj.TimescaleFinish field

Tanggal ketika skala waktu dalam tampilan berakhir.

```csharp
public static readonly Key<DateTime, PrjKey> TimescaleFinish;
```

## Contoh

Menampilkan cara membaca/menulis properti Prj.TimescaleFinish.

```csharp
var project = new Project();

project.Set(Prj.TimescaleFinish, new DateTime(2020, 4, 10, 9, 0, 0));

Console.WriteLine("Timescale Finish: " + project.Get(Prj.TimescaleFinish));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


