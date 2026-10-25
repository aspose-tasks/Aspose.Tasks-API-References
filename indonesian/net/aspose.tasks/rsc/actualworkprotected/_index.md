---
title: "Rsc.ActualWorkProtected"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Rsc. Jumlah pekerjaan yang melindungi pekerjaan aktual"
type: docs
weight: 80
url: /id/net/aspose.tasks/rsc/actualworkprotected/
---
## Rsc.ActualWorkProtected field

Jumlah pekerjaan yang melindungi pekerjaan aktual.

```csharp
public static readonly Key<Duration, RscKey> ActualWorkProtected;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.ActualWorkProtected.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Work Protected: " + resource.Get(Rsc.ActualWorkProtected));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


