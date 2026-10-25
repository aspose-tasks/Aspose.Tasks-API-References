---
title: "Asn.BCWP"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Asn field. Biaya yang dianggarkan untuk pekerjaan yang dilakukan pada penugasan hingga saat ini"
type: docs
weight: 120
url: /id/net/aspose.tasks/asn/bcwp/
---
## Asn.BCWP field

Biaya yang dianggarkan untuk pekerjaan yang dilakukan pada penugasan hingga saat ini.

```csharp
public static readonly Key<double, AsnKey> BCWP;
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


