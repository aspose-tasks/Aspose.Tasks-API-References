---
title: "Rsc.ActualWork"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Rsc. Jumlah pekerjaan yang telah selesai dilakukan oleh sumber daya yang ditugaskan ke tugas"
type: docs
weight: 70
url: /id/net/aspose.tasks/rsc/actualwork/
---
## Rsc.ActualWork field

Jumlah pekerjaan yang sudah selesai oleh sumber daya yang ditugaskan ke tugas.

```csharp
public static readonly Key<Duration, RscKey> ActualWork;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.ActualWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualWork, project.GetWork(1));

Console.WriteLine("Actual Work: " + resource.Get(Rsc.ActualWork));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


