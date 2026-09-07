---
title: "Rsc.SV"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Rsc. Varians jadwal nilai yang diperoleh hingga tanggal status proyek. SV adalah selisih antara biaya terbudgetkan dari pekerjaan yang dilakukan (BCWP) dan biaya terbudgetkan dari pekerjaan yang dijadwalkan (BCWS)"
type: docs
weight: 650
url: /id/net/aspose.tasks/rsc/sv/
---
## Rsc.SV field

Varians jadwal nilai yang diperoleh, hingga tanggal status proyek. SV adalah selisih antara biaya anggaran pekerjaan yang dilakukan (BCWP) dan biaya anggaran pekerjaan yang dijadwalkan (BCWS).

```csharp
public static readonly Key<double, RscKey> SV;
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


