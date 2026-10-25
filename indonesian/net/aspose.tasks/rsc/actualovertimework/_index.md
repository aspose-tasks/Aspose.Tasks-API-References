---
title: "Rsc.ActualOvertimeWork"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Rsc. Jumlah aktual pekerjaan lembur yang sudah dilakukan oleh sumber daya yang ditugaskan pada tugas"
type: docs
weight: 50
url: /id/net/aspose.tasks/rsc/actualovertimework/
---
## Rsc.ActualOvertimeWork field

Jumlah aktual lembur yang sudah dilakukan oleh sumber daya yang ditugaskan ke tugas.

```csharp
public static readonly Key<Duration, RscKey> ActualOvertimeWork;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.ActualOvertimeWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualOvertimeWork, project.GetWork(1));

Console.WriteLine("Actual Overtime Work: " + resource.Get(Rsc.ActualOvertimeWork));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


