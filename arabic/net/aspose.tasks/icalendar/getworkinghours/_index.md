---
title: "ICalendar.GetWorkingHours"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ICalendar. تُرجع WorkUnit بدء وانتهاء ومدة ساعات العمل للفترة الزمنية المحددة."
type: docs
weight: 60
url: /ar/net/aspose.tasks/icalendar/getworkinghours/
---
## GetWorkingHours(DateTime, DateTime) {#getworkinghours}

يرجع WorkUnit - بداية، انتهاء ومدة ساعات العمل للفترة الزمنية المحددة.

```csharp
public WorkUnit GetWorkingHours(DateTime start, DateTime finish)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| بداية | DateTime | تاريخ البدء للفترة. |
| انتهاء | DateTime | تاريخ الانتهاء للفترة. |

### قيمة الإرجاع

مثيل من فئة [`WorkUnit`](../../workunit/) يحتوي على بدء وانتهاء ومدة ساعات العمل.

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

* class [WorkUnit](../../workunit/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetWorkingHours(DateTime) {#getworkinghours_1}

يرجع مقدار ساعات العمل في التاريخ المحدد.

```csharp
public TimeSpan GetWorkingHours(DateTime dt)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| dt | DateTime | التاريخ للحصول على ساعات العمل. |

### قيمة الإرجاع

ساعات العمل في التاريخ المحدد.

### انظر أيضًا

* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


