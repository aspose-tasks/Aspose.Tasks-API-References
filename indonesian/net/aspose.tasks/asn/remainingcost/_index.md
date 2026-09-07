---
title: "Asn.RemainingCost"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Asn. Biaya proyeksi sisa untuk menyelesaikan sebuah penugasan"
type: docs
weight: 430
url: /id/net/aspose.tasks/asn/remainingcost/
---
## Asn.RemainingCost field

Biaya proyeksi tersisa untuk menyelesaikan sebuah penugasan.

```csharp
public static readonly Key<decimal, AsnKey> RemainingCost;
```

## Contoh

Menampilkan cara membaca lembur/pekerjaan/biaya yang tersisa dari sebuah penugasan.

```csharp
var project = new Project(DataDir + "ResourceAssignmentOvertimes.mpp");

// Cetak lembur penugasan
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.OvertimeWork).ToString());
    Console.WriteLine(ra.Get(Asn.OvertimeCost));
    Console.WriteLine(ra.Get(Asn.RemainingWork).ToString());
    Console.WriteLine(ra.Get(Asn.RemainingCost));
    Console.WriteLine(ra.Get(Asn.RemainingOvertimeWork).ToString());
    Console.WriteLine(ra.Get(Asn.RemainingOvertimeCost));
}
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


