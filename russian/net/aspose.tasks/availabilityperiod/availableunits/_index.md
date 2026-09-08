---
title: "AvailabilityPeriod.AvailableUnits"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство AvailabilityPeriod. Возвращает или задает процент ресурса, доступного в указанный период"
type: docs
weight: 40
url: /ru/net/aspose.tasks/availabilityperiod/availableunits/
---
## AvailabilityPeriod.AvailableUnits property

Получает или задает процент ресурса, доступного в течение указанного периода.

```csharp
public double AvailableUnits { get; set; }
```

## Примеры

Показывает, как создать периоды доступности для ресурса.

```csharp
public void WorkWithAvailabilityPeriod()
{
    var project = new Project();
    var resource = project.Resources.Add("Work Resource");

    // Добавить периоды доступности к новому ресурсу
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

### См. также

* class [AvailabilityPeriod](../)
* namespace [Aspose.Tasks](../../availabilityperiod/)
* assembly [Aspose.Tasks](../../../)


