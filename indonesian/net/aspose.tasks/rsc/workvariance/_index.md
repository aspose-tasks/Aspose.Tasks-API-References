---
title: "Rsc.WorkVariance"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Rsc. Perbedaan antara pekerjaan dasar sumber daya dan pekerjaan yang dijadwalkan saat ini"
type: docs
weight: 710
url: /id/net/aspose.tasks/rsc/workvariance/
---
## Rsc.WorkVariance field

Perbedaan antara pekerjaan baseline sebuah sumber daya dan pekerjaan yang saat ini dijadwalkan.

```csharp
public static readonly Key<double, RscKey> WorkVariance;
```

## Contoh

Menampilkan cara membaca varians pekerjaan sumber daya.

```csharp
var project = new Project(DataDir + "WorkVariance.mpp");

foreach (var assignment in project.ResourceAssignments)
{
    var resource = assignment.Get(Asn.Resource);

    var workVariance = resource.Get(Rsc.WorkVariance);

    Console.WriteLine(workVariance);
}
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


