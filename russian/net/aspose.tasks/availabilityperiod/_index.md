---
title: "Класс AvailabilityPeriod"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.AvailabilityPeriod. Представляет период, когда ресурс доступен"
type: docs
weight: 80
url: /ru/net/aspose.tasks/availabilityperiod/
---
## AvailabilityPeriod class

Представляет период, когда ресурс доступен.

```csharp
public class AvailabilityPeriod
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [AvailabilityPeriod](availabilityperiod/#constructor)() | Инициализирует новый экземпляр `AvailabilityPeriod`. |
| [AvailabilityPeriod](availabilityperiod/#constructor_1)(DateTime, DateTime, double) | Инициализирует новый экземпляр `AvailabilityPeriod` с указанным диапазоном дат и доступными единицами. |

## Свойства

| Имя | Описание |
| --- | --- |
| [AvailableFrom](../../aspose.tasks/availabilityperiod/availablefrom/) { get; set; } | Получает или задает дату, когда ресурс становится доступным для указанного периода. |
| [AvailableTo](../../aspose.tasks/availabilityperiod/availableto/) { get; set; } | Получает или задает последнюю дату, когда ресурс доступен для указанного периода. |
| [AvailableUnits](../../aspose.tasks/availabilityperiod/availableunits/) { get; set; } | Получает или задает процент ресурса, доступного в течение указанного периода. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


