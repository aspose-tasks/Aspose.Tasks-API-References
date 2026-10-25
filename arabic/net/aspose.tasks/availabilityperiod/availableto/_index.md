---
title: "AvailabilityPeriod.AvailableTo"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية AvailabilityPeriod. تحصل أو تعين آخر تاريخ يكون فيه المورد متاحًا للفترة المحددة"
type: docs
weight: 30
url: /ar/net/aspose.tasks/availabilityperiod/availableto/
---
## AvailabilityPeriod.AvailableTo property

يحصل أو يضبط آخر تاريخ يكون فيه المورد متاحًا للفترة المحددة.

```csharp
public DateTime AvailableTo { get; set; }
```

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

* class [AvailabilityPeriod](../)
* namespace [Aspose.Tasks](../../availabilityperiod/)
* assembly [Aspose.Tasks](../../../)


