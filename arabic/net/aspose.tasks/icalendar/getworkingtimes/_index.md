---
title: "ICalendar.GetWorkingTimes"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ICalendar. تُرجع WorkingTimeCollection لأوقات العمل للتاريخ المحدد"
type: docs
weight: 80
url: /ar/net/aspose.tasks/icalendar/getworkingtimes/
---
## ICalendar.GetWorkingTimes method

تُرجع [`WorkingTimeCollection`](../../workingtimecollection/) لأوقات العمل للتاريخ المحدد.

```csharp
public WorkingTimeCollection GetWorkingTimes(DateTime dt)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| dt | DateTime | التاريخ للحصول على أوقات العمل. |

### قيمة الإرجاع

مجموعة من مثيلات [`WorkingTime`](../../workingtime/).

## الأمثلة

يوضح كيفية استخدام طريقة Calendar.GetIntersectionCalendar() لإجراء حساب على تقويم المهمة.

```csharp
var project = new Project(DataDir + "CalculateWorkHours.mpp");

foreach (var ra in project.ResourceAssignments)
{
    if (ra.Resource == null)
    {
        continue;
    }

    ICalendar assignmentCalendar;

    Calendar taskCalendar = ra.Task.Calendar != null && !ra.Task.Duration.IsEstimated ? ra.Task.Calendar : null;
    Calendar resourceCalendar = ra.Resource.Calendar != null && !ra.Task.IgnoreResourceCalendar
        ? ra.Resource.Calendar
        : null;

    if (taskCalendar != null && resourceCalendar != null && !ReferenceEquals(taskCalendar, resourceCalendar))
    {
        assignmentCalendar = Calendar.GetIntersectionCalendar(taskCalendar, resourceCalendar);
    }
    else
    {
        assignmentCalendar = taskCalendar ?? resourceCalendar;
    }

    if (assignmentCalendar == null)
    {
        assignmentCalendar = project.Calendar;
    }

    var workingHours = assignmentCalendar.GetWorkingHours(ra.Start, ra.Finish);

    Console.WriteLine("Working hours for assignment '{0}' : {1}", ra, workingHours);

    var date = new DateTime(2025, 4, 7);
    Console.WriteLine("Working times for date '{0}':", date);

    foreach (var wt in assignmentCalendar.GetWorkingTimes(date))
    {
        Console.WriteLine("{0} - {1}", wt.From.TimeOfDay, wt.To.TimeOfDay);
    }
}
```

### انظر أيضًا

* class [WorkingTimeCollection](../../workingtimecollection/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


