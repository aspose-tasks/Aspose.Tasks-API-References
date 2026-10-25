---
title: "Asn.SV"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Asn. Varians jadwal nilai yang diperoleh hingga tanggal status proyek. Varians jadwal SV adalah selisih antara BCWP dan BCWS"
type: docs
weight: 540
url: /id/net/aspose.tasks/asn/sv/
---
## Asn.SV field

Variansi jadwal nilai yang diperoleh, hingga tanggal status proyek. Variansi jadwal (SV) adalah selisih antara BCWP dan BCWS.

```csharp
public static readonly Key<double, AsnKey> SV;
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


