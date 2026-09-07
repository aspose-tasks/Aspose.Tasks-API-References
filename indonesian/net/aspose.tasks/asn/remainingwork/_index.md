---
title: "Asn.RemainingWork"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Asn. Pekerjaan tersisa yang dijadwalkan untuk menyelesaikan sebuah penugasan"
type: docs
weight: 460
url: /id/net/aspose.tasks/asn/remainingwork/
---
## Asn.RemainingWork field

Pekerjaan tersisa yang dijadwalkan untuk menyelesaikan sebuah penugasan.

```csharp
public static readonly Key<Duration, AsnKey> RemainingWork;
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
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


