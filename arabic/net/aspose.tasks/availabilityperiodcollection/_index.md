---
title: "الفئة AvailabilityPeriodCollection"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.AvailabilityPeriodCollection. تمثل مجموعة تحتوي على كائنات AvailabilityPeriod"
type: docs
weight: 90
url: /ar/net/aspose.tasks/availabilityperiodcollection/
---
## AvailabilityPeriodCollection class

تمثل مجموعة تحتوي على كائنات [`AvailabilityPeriod`](../availabilityperiod/).

```csharp
public class AvailabilityPeriodCollection : IList<AvailabilityPeriod>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Count](../../aspose.tasks/availabilityperiodcollection/count/) { get; } | يحصل على عدد العناصر الموجودة في هذه المجموعة. |
| [IsReadOnly](../../aspose.tasks/availabilityperiodcollection/isreadonly/) { get; } | يحصل على قيمة تشير إلى ما إذا كانت هذه المجموعة للقراءة فقط؛ وإلا، false. |
| [Item](../../aspose.tasks/availabilityperiodcollection/item/) { get; set; } | يرجع أو يعيّن العنصر في الفهرس المحدد. |
| [ParentResource](../../aspose.tasks/availabilityperiodcollection/parentresource/) { get; } | يحصل على العنصر الأب [`Resource`](../resource/) لهذا الكائن. العنصر الأب [`Resource`](../resource/) لهذه المجموعة. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.tasks/availabilityperiodcollection/add/)(AvailabilityPeriod) | يضيف العنصر المحدد إلى هذه المجموعة. |
| [Clear](../../aspose.tasks/availabilityperiodcollection/clear/)() | يزيل جميع العناصر من هذه المجموعة. |
| [Contains](../../aspose.tasks/availabilityperiodcollection/contains/)(AvailabilityPeriod) | يرجع true إذا تم العثور على العنصر المحدد في هذه المجموعة؛ وإلا، false. |
| [CopyTo](../../aspose.tasks/availabilityperiodcollection/copyto/)(AvailabilityPeriod[], int) | ينسخ عناصر هذه المجموعة إلى المصفوفة المحددة، بدءًا من الفهرس المحدد للمصفوفة. |
| [GetEnumerator](../../aspose.tasks/availabilityperiodcollection/getenumerator/)() | يرجع عدادًا لهذه المجموعة. |
| [IndexOf](../../aspose.tasks/availabilityperiodcollection/indexof/)(AvailabilityPeriod) | يحدد فهرس العنصر المحدد في هذه المجموعة. |
| [Insert](../../aspose.tasks/availabilityperiodcollection/insert/)(int, AvailabilityPeriod) | يدرج العنصر المحدد في الفهرس المحدد. |
| [Remove](../../aspose.tasks/availabilityperiodcollection/remove/)(AvailabilityPeriod) | يزيل الظهور الأول لكائن محدد من هذه المجموعة. |
| [RemoveAt](../../aspose.tasks/availabilityperiodcollection/removeat/)(int) | يزيل عنصرًا في الفهرس المحدد. |

## الأمثلة

يوضح كيفية العمل مع مجموعة فترات التوافر للموارد.

```csharp
public void WorkWithAvailabilityPeriodCollection()
{
    var project = new Project(DataDir + "UpdateResourceData.mpp");
    var resource = project.Resources.GetById(1);

    resource.AvailabilityPeriods.Clear();

    // أضف فترات التوافر (سنتا 2012 و 2014) إلى المورد الجديد
    IEnumerable<AvailabilityPeriod> periods = this.GetPeriods();
    foreach (var period in periods)
    {
        if (!resource.AvailabilityPeriods.IsReadOnly)
        {
            resource.AvailabilityPeriods.Add(period);
        }
    }

    var period2013 = new AvailabilityPeriod { AvailableFrom = new DateTime(2013, 1, 1), AvailableTo = new DateTime(2013, 12, 12), AvailableUnits = 0.81 };

    if (!resource.AvailabilityPeriods.Contains(period2013))
    {
        resource.AvailabilityPeriods.Insert(1, period2013);
    }

    Console.WriteLine("Count of availability periods: " + resource.AvailabilityPeriods.Count);
    foreach (var period in resource.AvailabilityPeriods)
    {
        Console.WriteLine("Available From: " + period.AvailableFrom);
        Console.WriteLine("Available To: " + period.AvailableTo);
        Console.WriteLine("Available Units: " + period.AvailableUnits);
        Console.WriteLine();
    }

    var periodsToCopy = new AvailabilityPeriod[resource.AvailabilityPeriods.Count];
    resource.AvailabilityPeriods.CopyTo(periodsToCopy, 0);

    var otherResource = project.Resources.GetById(2);
    otherResource.AvailabilityPeriods.Clear();
    foreach (var period in periodsToCopy)
    {
        otherResource.AvailabilityPeriods.Add(period);
    }

    var period2015 = new AvailabilityPeriod { AvailableFrom = new DateTime(2015, 1, 1), AvailableTo = new DateTime(2015, 12, 12), AvailableUnits = 0.50 };

    var period2016 = new AvailabilityPeriod { AvailableFrom = new DateTime(2016, 1, 1), AvailableTo = new DateTime(2016, 12, 12), AvailableUnits = 0.53 };

    if (otherResource.AvailabilityPeriods.IndexOf(period2015) < 0)
    {
        otherResource.AvailabilityPeriods.Add(period2015);
    }

    if (otherResource.AvailabilityPeriods.IndexOf(period2016) < 0)
    {
        otherResource.AvailabilityPeriods.Add(period2016);
    }

    // تحديث الوحدات المتاحة للفترة لعام 2014
    otherResource.AvailabilityPeriods[otherResource.AvailabilityPeriods.Count - 2].AvailableUnits = 0.90;

    // إزالة الفترة لعام 2013
    otherResource.AvailabilityPeriods.Remove(period2013);

    // إزالة الفترة لعام 2011
    otherResource.AvailabilityPeriods.RemoveAt(0);

    Console.WriteLine("Print resource availability periods of the resource: " + otherResource.Get(Rsc.Name));
    Console.WriteLine("Count of availability periods: " + resource.AvailabilityPeriods.Count);
    foreach (var period in resource.AvailabilityPeriods)
    {
        Console.WriteLine("Available From: " + period.AvailableFrom);
        Console.WriteLine("Available To: " + period.AvailableTo);
        Console.WriteLine("Available Units: " + period.AvailableUnits);
        Console.WriteLine();
    }
}

private IEnumerable<AvailabilityPeriod> GetPeriods()
{
    var periods = new List<AvailabilityPeriod>();
    var period = new AvailabilityPeriod { AvailableFrom = new DateTime(2012, 1, 1), AvailableTo = new DateTime(2012, 12, 12), AvailableUnits = 0.99 };
    periods.Add(period);

    var period2 = new AvailabilityPeriod { AvailableFrom = new DateTime(2014, 1, 1), AvailableTo = new DateTime(2014, 12, 12), AvailableUnits = 0.94 };
    periods.Add(period2);
    return periods;
}
```

### انظر أيضًا

* class [AvailabilityPeriod](../availabilityperiod/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


