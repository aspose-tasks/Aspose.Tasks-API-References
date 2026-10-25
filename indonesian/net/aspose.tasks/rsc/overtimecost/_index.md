---
title: "Rsc.OvertimeCost"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Rsc field. Total biaya lembur untuk sebuah sumber daya pada semua tugas yang ditugaskan"
type: docs
weight: 500
url: /id/net/aspose.tasks/rsc/overtimecost/
---
## Rsc.OvertimeCost field

Total biaya lembur untuk sumber daya pada semua tugas yang ditugaskan.

```csharp
public static readonly Key<decimal, RscKey> OvertimeCost;
```

## Contoh

Menampilkan cara membaca nilai lembur sumber daya.

```csharp
var project = new Project(DataDir + "ResourceOvertime.mpp");

// Tampilkan parameter terkait lembur untuk semua sumber daya
foreach (var res in project.Resources)
{
    if (res.Get(Rsc.Name) == null)
    {
        continue;
    }

    Console.WriteLine(res.Get(Rsc.OvertimeCost));
    Console.WriteLine(res.Get(Rsc.OvertimeWork).ToString());
    Console.WriteLine(res.Get(Rsc.OvertimeRateFormat).ToString());
}
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


