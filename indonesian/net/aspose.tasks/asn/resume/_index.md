---
title: "Asn.Resume"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Asn. Tanggal ketika penugasan dilanjutkan."
type: docs
weight: 490
url: /id/net/aspose.tasks/asn/resume/
---
## Asn.Resume field

Tanggal ketika penugasan dilanjutkan.

```csharp
public static readonly Key<DateTime, AsnKey> Resume;
```

## Contoh

Menampilkan cara membaca tanggal berhenti/lanjut penugasan.

```csharp
var project = new Project(DataDir + "ResourceAssignmentStopResumeDates.mpp");

// Cetak tanggal berhenti dan melanjutkan penugasan sumber daya
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.Stop).ToShortDateString() == "1/1/2000" ? "NA" : ra.Get(Asn.Stop).ToShortDateString());
    Console.WriteLine(ra.Get(Asn.Resume).ToShortDateString() == "1/1/2000" ? "NA" : ra.Get(Asn.Resume).ToShortDateString());
}
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


