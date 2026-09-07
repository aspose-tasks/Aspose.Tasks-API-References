---
title: "Asn.StartVariance"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Asn. Varians tanggal mulai penugasan dari tanggal mulai dasar"
type: docs
weight: 510
url: /id/net/aspose.tasks/asn/startvariance/
---
## Asn.StartVariance field

Variansi tanggal mulai penugasan dari tanggal mulai baseline.

```csharp
public static readonly Key<Duration, AsnKey> StartVariance;
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


