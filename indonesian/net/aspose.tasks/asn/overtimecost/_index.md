---
title: "Asn.OvertimeCost"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Asn. Jumlah biaya lembur aktual dan sisa dari sebuah penugasan"
type: docs
weight: 370
url: /id/net/aspose.tasks/asn/overtimecost/
---
## Asn.OvertimeCost field

Jumlah biaya lembur aktual dan sisa lembur dari sebuah penugasan.

```csharp
public static readonly Key<decimal, AsnKey> OvertimeCost;
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


