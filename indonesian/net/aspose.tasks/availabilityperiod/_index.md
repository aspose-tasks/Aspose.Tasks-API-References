---
title: "Kelas AvailabilityPeriod"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.AvailabilityPeriod. Mewakili periode ketika sumber daya tersedia"
type: docs
weight: 80
url: /id/net/aspose.tasks/availabilityperiod/
---
## AvailabilityPeriod class

Mewakili periode ketika sumber daya tersedia.

```csharp
public class AvailabilityPeriod
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [AvailabilityPeriod](availabilityperiod/#constructor)() | Menginisialisasi instance baru dari `AvailabilityPeriod`. |
| [AvailabilityPeriod](availabilityperiod/#constructor_1)(DateTime, DateTime, double) | Menginisialisasi instance baru dari `AvailabilityPeriod` dengan rentang tanggal dan unit yang tersedia yang ditentukan. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [AvailableFrom](../../aspose.tasks/availabilityperiod/availablefrom/) { get; set; } | Mendapatkan atau mengatur tanggal ketika sumber daya menjadi tersedia untuk periode yang ditentukan. |
| [AvailableTo](../../aspose.tasks/availabilityperiod/availableto/) { get; set; } | Mendapatkan atau mengatur tanggal terakhir ketika sumber daya tersedia untuk periode yang ditentukan. |
| [AvailableUnits](../../aspose.tasks/availabilityperiod/availableunits/) { get; set; } | Mendapatkan atau mengatur persentase sumber daya yang tersedia selama periode yang ditentukan. |

## Contoh

Menampilkan cara membuat periode ketersediaan untuk sebuah sumber daya.

```csharp
public void WorkWithAvailabilityPeriod()
{
    var project = new Project();
    var resource = project.Resources.Add("Work Resource");

    // Tambahkan periode ketersediaan ke sumber daya baru
    IEnumerable<AvailabilityPeriod> periods = GetPeriods();
    foreach (var period in periods)
    {
        resource.AvailabilityPeriods.Add(period);
    }

    foreach (var period in resource.AvailabilityPeriods)
    {
        Console.WriteLine("Available From: " + period.AvailableFrom);
        Console.WriteLine("Available To: " + period.AvailableTo);
        Console.WriteLine("Available Units: " + period.AvailableUnits);
        Console.WriteLine();
    }
}

private static IEnumerable<AvailabilityPeriod> GetPeriods()
{
    var periods = new List<AvailabilityPeriod>(2);
    var period = new AvailabilityPeriod
    {
        AvailableFrom = new DateTime(2011, 12, 12),
        AvailableTo = new DateTime(2013, 12, 12),
        AvailableUnits = 0.99
    };

    periods.Add(period);

    var period2 = new AvailabilityPeriod
    {
        AvailableFrom = new DateTime(2013, 12, 12),
        AvailableTo = new DateTime(2015, 12, 12),
        AvailableUnits = 0.94
    };
    periods.Add(period2);
    return periods;
}
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


