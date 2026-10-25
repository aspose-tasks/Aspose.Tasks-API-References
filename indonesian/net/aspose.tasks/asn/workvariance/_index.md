---
title: "Asn.WorkVariance"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Asn. Perbedaan antara pekerjaan dasar sebuah tugas dan pekerjaan yang saat ini dijadwalkan"
type: docs
weight: 620
url: /id/net/aspose.tasks/asn/workvariance/
---
## Asn.WorkVariance field

Selisih antara pekerjaan baseline sebuah tugas dan pekerjaan yang dijadwalkan saat ini.

```csharp
public static readonly Key<Duration, AsnKey> WorkVariance;
```

## Contoh

Menampilkan cara membaca varians penugasan.

```csharp
var project = new Project(DataDir + "ResourceAssignmentVariance.mpp");

// Cetak varians penugasan
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.WorkVariance));
    Console.WriteLine(ra.Get(Asn.CostVariance));
    Console.WriteLine(ra.Get(Asn.StartVariance));
    Console.WriteLine(ra.Get(Asn.FinishVariance));
}
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


