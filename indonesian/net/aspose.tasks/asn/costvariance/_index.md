---
title: "Asn.CostVariance"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Asn. Perbedaan antara biaya dasar dan total biaya untuk sebuah penugasan"
type: docs
weight: 200
url: /id/net/aspose.tasks/asn/costvariance/
---
## Asn.CostVariance field

Perbedaan antara biaya dasar dan total biaya untuk sebuah penugasan.

```csharp
public static readonly Key<double, AsnKey> CostVariance;
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
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


