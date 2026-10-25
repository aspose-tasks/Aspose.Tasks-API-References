---
title: "فئة AvailabilityPeriod"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Aspose.Tasks.AvailabilityPeriod class. يمثل فترة يكون فيها المورد متاحًا"
type: docs
weight: 80
url: /ar/net/aspose.tasks/availabilityperiod/
---
## AvailabilityPeriod class

يمثل فترة يكون فيها المورد متاحًا.

```csharp
public class AvailabilityPeriod
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [AvailabilityPeriod](availabilityperiod/#constructor)() | ينشئ مثيلًا جديدًا من `AvailabilityPeriod`. |
| [AvailabilityPeriod](availabilityperiod/#constructor_1)(DateTime, DateTime, double) | ينشئ مثيلًا جديدًا من `AvailabilityPeriod` بالنطاق الزمني المحدد والوحدات المتاحة. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AvailableFrom](../../aspose.tasks/availabilityperiod/availablefrom/) { get; set; } | يحصل أو يضبط التاريخ الذي يصبح فيه المورد متاحًا للفترة المحددة. |
| [AvailableTo](../../aspose.tasks/availabilityperiod/availableto/) { get; set; } | يحصل أو يضبط آخر تاريخ يكون فيه المورد متاحًا للفترة المحددة. |
| [AvailableUnits](../../aspose.tasks/availabilityperiod/availableunits/) { get; set; } | يحصل أو يضبط نسبة المورد المتاح خلال الفترة المحددة. |

## الأمثلة

يوضح كيفية إنشاء فترات التوافر لمورد.

```csharp
public void WorkWithAvailabilityPeriod()
{
    var project = new Project();
    var resource = project.Resources.Add("Work Resource");

    // إضافة فترات التوافر إلى مورد جديد
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

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


