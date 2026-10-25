---
title: "Class AvailabilityPeriod"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.AvailabilityPeriod class. Bir kaynağın mevcut olduğu bir dönemi temsil eder"
type: docs
weight: 80
url: /tr/net/aspose.tasks/availabilityperiod/
---
## AvailabilityPeriod class

Bir kaynağın mevcut olduğu bir dönemi temsil eder.

```csharp
public class AvailabilityPeriod
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [AvailabilityPeriod](availabilityperiod/#constructor)() | Yeni bir `AvailabilityPeriod` örneği başlatır. |
| [AvailabilityPeriod](availabilityperiod/#constructor_1)(DateTime, DateTime, double) | Belirtilen tarih aralığı ve mevcut birimlerle yeni bir `AvailabilityPeriod` örneği başlatır. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AvailableFrom](../../aspose.tasks/availabilityperiod/availablefrom/) { get; set; } | Belirtilen dönem için bir kaynağın kullanılabilir hale geldiği tarihi alır veya ayarlar. |
| [AvailableTo](../../aspose.tasks/availabilityperiod/availableto/) { get; set; } | Belirtilen dönem için bir kaynağın kullanılabilir olduğu son tarihi alır veya ayarlar. |
| [AvailableUnits](../../aspose.tasks/availabilityperiod/availableunits/) { get; set; } | Belirtilen dönem boyunca bir kaynağın kullanılabilir olduğu yüzdeyi alır veya ayarlar. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


