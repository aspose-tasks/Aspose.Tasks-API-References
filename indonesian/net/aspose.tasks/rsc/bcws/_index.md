---
title: "Rsc.BCWS"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Rsc field. Biaya anggaran pekerjaan yang dijadwalkan untuk sebuah sumber daya"
type: docs
weight: 150
url: /id/net/aspose.tasks/rsc/bcws/
---
## Rsc.BCWS field

Biaya anggaran dari pekerjaan yang dijadwalkan untuk sumber daya.

```csharp
public static readonly Key<double, RscKey> BCWS;
```

## Contoh

Menampilkan cara membaca biaya sumber daya.

```csharp
var project = new Project(DataDir + "ResourceCosts.mpp");

// Tampilkan semua biaya sumber daya
foreach (var res in project.Resources)
{
    if (res.Get(Rsc.Name) == null)
    {
        continue;
    }

    Console.WriteLine(res.Get(Rsc.Cost));
    Console.WriteLine(res.Get(Rsc.ACWP));
    Console.WriteLine(res.Get(Rsc.BCWS));
    Console.WriteLine(res.Get(Rsc.BCWP));

    // CV = BCWP - ACWP
    Console.WriteLine(res.Get(Rsc.CV));

    // SV = BCWP - BCWS
    Console.WriteLine(res.Get(Rsc.SV));
}
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


