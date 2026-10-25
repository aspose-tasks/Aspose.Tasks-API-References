---
title: "Asn.CV"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Asn. Varians biaya nilai yang diperoleh. CV adalah selisih antara BCWP (biaya anggaran pekerjaan yang selesai) penugasan dan ACWP (biaya aktual pekerjaan yang selesai)."
type: docs
weight: 220
url: /id/net/aspose.tasks/asn/cv/
---
## Asn.CV field

Varians biaya nilai yang diperoleh. CV adalah perbedaan antara BCWP (biaya yang dianggarkan untuk pekerjaan yang dilakukan) penugasan dan ACWP (biaya aktual pekerjaan yang dilakukan).

```csharp
public static readonly Key<double, AsnKey> CV;
```

## Contoh

Menampilkan cara membaca nilai biaya penugasan.

```csharp
var project = new Project(DataDir + "ResourceAssignmentCosts.mpp");

// Cetak biaya penugasan sumber daya
foreach (var assignment in project.ResourceAssignments)
{
    Console.WriteLine(assignment.Get(Asn.Cost));
    Console.WriteLine(assignment.Get(Asn.ACWP));

    // CV = BCWP - ACWP
    Console.WriteLine(assignment.Get(Asn.CV));

    Console.WriteLine(assignment.Get(Asn.BCWP));
    Console.WriteLine(assignment.Get(Asn.BCWS));

    // SV = BCWP - BCWS
    Console.WriteLine(assignment.Get(Asn.SV));
}
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


