---
title: "Rsc.OvertimeRateFormat"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Rsc. Unit yang digunakan oleh Microsoft Project untuk menampilkan tarif lembur"
type: docs
weight: 520
url: /id/net/aspose.tasks/rsc/overtimerateformat/
---
## Rsc.OvertimeRateFormat field

Satuan yang digunakan Microsoft Project untuk menampilkan tarif lembur.

```csharp
public static readonly Key<RateFormatType, RscKey> OvertimeRateFormat;
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
* enum [RateFormatType](../../rateformattype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


