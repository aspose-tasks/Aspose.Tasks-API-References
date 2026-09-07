---
title: "Rsc.RemainingOvertimeWork"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Rsc field. Jumlah lembur terjadwal yang tersisa"
type: docs
weight: 600
url: /id/net/aspose.tasks/rsc/remainingovertimework/
---
## Rsc.RemainingOvertimeWork field

Jumlah lembur terjadwal yang tersisa.

```csharp
public static readonly Key<Duration, RscKey> RemainingOvertimeWork;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.RemainingOvertimeWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingOvertimeWork, project.GetWork(1));

Console.WriteLine("Remaining Overtime Work: " + resource.Get(Rsc.RemainingOvertimeWork));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


