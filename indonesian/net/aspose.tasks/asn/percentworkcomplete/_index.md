---
title: "Asn.PercentWorkComplete"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Asn. Jumlah pekerjaan yang selesai pada sebuah penugasan"
type: docs
weight: 400
url: /id/net/aspose.tasks/asn/percentworkcomplete/
---
## Asn.PercentWorkComplete field

Jumlah pekerjaan yang selesai pada sebuah penugasan.

```csharp
public static readonly Key<int, AsnKey> PercentWorkComplete;
```

## Contoh

Menampilkan cara membaca persentase pekerjaan selesai dari sebuah penugasan.

```csharp
var project = new Project(DataDir + "ResourceAssignmentPercentWorkComplete.mpp");

// Cetak persentase penyelesaian penugasan
foreach (var ra in project.ResourceAssignments)
{
    Console.WriteLine(ra.Get(Asn.PercentWorkComplete).ToString());
}
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


