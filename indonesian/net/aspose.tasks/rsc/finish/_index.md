---
title: "Rsc.Finish"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Rsc. Tanggal ketika sebuah sumber daya dijadwalkan menyelesaikan pekerjaan pada semua tugas yang ditugaskan"
type: docs
weight: 290
url: /id/net/aspose.tasks/rsc/finish/
---
## Rsc.Finish field

Tanggal ketika sumber daya dijadwalkan menyelesaikan pekerjaan pada semua tugas yang ditugaskan.

```csharp
public static readonly Key<DateTime, RscKey> Finish;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.Finish.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Finish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Finish: " + resource.Get(Rsc.Finish));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


