---
title: "Rsc.Start"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Rsc. Tanggal ketika sumber daya yang ditugaskan dijadwalkan untuk mulai bekerja pada tugas"
type: docs
weight: 640
url: /id/net/aspose.tasks/rsc/start/
---
## Rsc.Start field

Tanggal ketika sumber daya yang ditugaskan dijadwalkan mulai bekerja pada sebuah tugas.

```csharp
public static readonly Key<DateTime, RscKey> Start;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.Start.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Start, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Start: " + resource.Get(Rsc.Start));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


