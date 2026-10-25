---
title: "Rsc.ActualOvertimeWorkProtected"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Rsc field. Jumlah pekerjaan di mana kerja lembur aktual dilindungi"
type: docs
weight: 60
url: /id/net/aspose.tasks/rsc/actualovertimeworkprotected/
---
## Rsc.ActualOvertimeWorkProtected field

Jumlah pekerjaan yang melindungi lembur aktual.

```csharp
public static readonly Key<Duration, RscKey> ActualOvertimeWorkProtected;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.ActualOvertimeWorkProtected.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualOvertimeWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Overtime Work Protected: " + resource.Get(Rsc.ActualOvertimeWorkProtected));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


