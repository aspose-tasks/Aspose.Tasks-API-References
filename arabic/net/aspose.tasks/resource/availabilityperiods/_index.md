---
title: "Resource.AvailabilityPeriods"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Resource. يحصل على نسخة من الفئة AvailabilityPeriodCollection. مجموعة الفترات التي يكون فيها المورد متاحًا"
type: docs
weight: 130
url: /ar/net/aspose.tasks/resource/availabilityperiods/
---
## Resource.AvailabilityPeriods property

يحصل على نسخة من الفئة [`AvailabilityPeriodCollection`](../../availabilityperiodcollection/) . مجموعة الفترات التي يكون فيها المورد متاحًا.

```csharp
public AvailabilityPeriodCollection AvailabilityPeriods { get; }
```

## الأمثلة

يوضح كيفية إضافة فترة توافر لمورد.

```csharp
var project = new Project();
var resource = project.Resources.Add("Resource");

var availabilityPeriod = new AvailabilityPeriod
{
    AvailableFrom = new DateTime(2020, 4, 1, 8, 0, 0),
    AvailableTo = new DateTime(2020, 4, 1, 17, 0, 0),
    AvailableUnits = 2d
};
resource.AvailabilityPeriods.Add(availabilityPeriod);

var availabilityPeriod2 = new AvailabilityPeriod
{
    AvailableFrom = new DateTime(2020, 4, 2, 8, 0, 0),
    AvailableTo = new DateTime(2020, 4, 2, 17, 0, 0),
    AvailableUnits = 3d
};
resource.AvailabilityPeriods.Add(availabilityPeriod2);
```

### انظر أيضًا

* class [AvailabilityPeriodCollection](../../availabilityperiodcollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


