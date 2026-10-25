---
title: "Rsc.Cost"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Rsc field. Total biaya terjadwal atau diproyeksikan untuk sebuah sumber daya berdasarkan biaya yang sudah dikeluarkan untuk pekerjaan yang dilakukan oleh sumber daya yang ditugaskan ke tugas, serta biaya yang direncanakan untuk pekerjaan yang tersisa"
type: docs
weight: 220
url: /id/net/aspose.tasks/rsc/cost/
---
## Rsc.Cost field

Total biaya terjadwal atau diproyeksikan untuk sumber daya, berdasarkan biaya yang sudah dikeluarkan untuk pekerjaan yang dilakukan oleh sumber daya yang ditugaskan ke tugas, serta biaya yang direncanakan untuk pekerjaan yang tersisa.

```csharp
public static readonly Key<decimal, RscKey> Cost;
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


