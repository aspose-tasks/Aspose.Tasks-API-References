---
title: "Rsc.Work"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Rsc. Jumlah total waktu yang dijadwalkan untuk sumber daya pada sebuah tugas"
type: docs
weight: 690
url: /id/net/aspose.tasks/rsc/work/
---
## Rsc.Work field

Jumlah total waktu yang dijadwalkan untuk sebuah sumber daya pada sebuah tugas.

```csharp
public static readonly Key<Duration, RscKey> Work;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.Work.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Work, project.GetWork(1));

Console.WriteLine("Work: " + resource.Get(Rsc.Work));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


