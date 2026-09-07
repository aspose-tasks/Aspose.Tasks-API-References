---
title: "Asn.BCWS"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Asn. Biaya yang dianggarkan untuk pekerjaan pada penugasan"
type: docs
weight: 130
url: /id/net/aspose.tasks/asn/bcws/
---
## Asn.BCWS field

Biaya yang dianggarkan untuk pekerjaan pada penugasan.

```csharp
public static readonly Key<double, AsnKey> BCWS;
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


