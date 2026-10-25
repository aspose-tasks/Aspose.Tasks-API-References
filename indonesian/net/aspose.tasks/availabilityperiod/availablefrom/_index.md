---
title: "AvailabilityPeriod.AvailableFrom"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti AvailabilityPeriod. Mendapatkan atau mengatur tanggal ketika sumber daya menjadi tersedia untuk periode yang ditentukan"
type: docs
weight: 20
url: /id/net/aspose.tasks/availabilityperiod/availablefrom/
---
## AvailabilityPeriod.AvailableFrom property

Mendapatkan atau mengatur tanggal ketika sumber daya menjadi tersedia untuk periode yang ditentukan.

```csharp
public DateTime AvailableFrom { get; set; }
```

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

* class [AvailabilityPeriod](../)
* namespace [Aspose.Tasks](../../availabilityperiod/)
* assembly [Aspose.Tasks](../../../)


