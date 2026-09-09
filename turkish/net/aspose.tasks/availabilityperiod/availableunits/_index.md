---
title: "AvailabilityPeriod.AvailableUnits"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "AvailabilityPeriod özelliği. Belirtilen dönemde bir kaynağın mevcut olduğu yüzdeyi alır veya ayarlar"
type: docs
weight: 40
url: /tr/net/aspose.tasks/availabilityperiod/availableunits/
---
## AvailabilityPeriod.AvailableUnits property

Belirtilen dönem boyunca bir kaynağın kullanılabilir olduğu yüzdeyi alır veya ayarlar.

```csharp
public double AvailableUnits { get; set; }
```

## Örnekler

Bir kaynak için kullanılabilirlik dönemlerinin nasıl oluşturulacağını gösterir.

```csharp
public void WorkWithAvailabilityPeriod()
{
    var project = new Project();
    var resource = project.Resources.Add("Work Resource");

    // Yeni kaynağa kullanılabilirlik dönemleri ekle
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

### Ayrıca Bakınız

* class [AvailabilityPeriod](../)
* namespace [Aspose.Tasks](../../availabilityperiod/)
* assembly [Aspose.Tasks](../../../)


