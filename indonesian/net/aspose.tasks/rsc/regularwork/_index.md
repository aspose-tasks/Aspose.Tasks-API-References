---
title: "Rsc.RegularWork"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Rsc. Jumlah total pekerjaan non lembur yang dijadwalkan untuk dilakukan oleh sumber daya"
type: docs
weight: 570
url: /id/net/aspose.tasks/rsc/regularwork/
---
## Rsc.RegularWork field

Jumlah total pekerjaan non lembur yang dijadwalkan untuk dilakukan oleh sumber daya.

```csharp
public static readonly Key<Duration, RscKey> RegularWork;
```

## Contoh

Menampilkan cara membaca/menulis properti Rsc.RegularWork.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RegularWork, project.GetWork(1));

Console.WriteLine("Regular Work: " + resource.Get(Rsc.RegularWork));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


