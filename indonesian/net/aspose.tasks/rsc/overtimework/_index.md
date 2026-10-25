---
title: "Rsc.OvertimeWork"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Rsc field. Jumlah lembur yang dijadwalkan untuk dilakukan oleh sebuah sumber daya pada sebuah tugas dan dikenakan tarif lembur sumber daya yang terlibat"
type: docs
weight: 530
url: /id/net/aspose.tasks/rsc/overtimework/
---
## Rsc.OvertimeWork field

Jumlah lembur yang dijadwalkan untuk dilakukan oleh sumber daya pada sebuah tugas dan dikenakan tarif lembur sumber daya yang terlibat.

```csharp
public static readonly Key<Duration, RscKey> OvertimeWork;
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
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


