---
title: "Asn.RemainingOvertimeCost"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Asn. Biaya lembur proyeksi yang tersisa untuk menyelesaikan penugasan."
type: docs
weight: 440
url: /id/net/aspose.tasks/asn/remainingovertimecost/
---
## Asn.RemainingOvertimeCost field

Biaya proyeksi lembur tersisa untuk menyelesaikan sebuah penugasan.

```csharp
public static readonly Key<decimal, AsnKey> RemainingOvertimeCost;
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


