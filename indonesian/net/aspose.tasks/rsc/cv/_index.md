---
title: "Rsc.CV"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Rsc. Varians biaya nilai yang diperoleh hingga tanggal status proyek. CV adalah perbedaan antara BCWP (biaya anggaran pekerjaan yang selesai) dan ACWP (biaya aktual pekerjaan yang selesai) pada tugas."
type: docs
weight: 270
url: /id/net/aspose.tasks/rsc/cv/
---
## Rsc.CV field

Varians biaya nilai yang diperoleh, hingga tanggal status proyek. CV adalah selisih antara BCWP (biaya anggaran pekerjaan yang dilakukan) dan ACWP (biaya aktual pekerjaan yang dilakukan) pada tugas.

```csharp
public static readonly Key<double, RscKey> CV;
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


