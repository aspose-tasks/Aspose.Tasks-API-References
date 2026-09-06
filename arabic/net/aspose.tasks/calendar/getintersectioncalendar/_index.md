---
title: "Calendar.GetIntersectionCalendar"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Calendar. تحصل على كائن ICalendar يمكن استخدامه لإجراء حسابات على تقاطع جداول عمل تقويمين"
type: docs
weight: 280
url: /ar/net/aspose.tasks/calendar/getintersectioncalendar/
---
## Calendar.GetIntersectionCalendar method

يحصل على كائن [`ICalendar`](../../icalendar/) يمكن استخدامه لإجراء حسابات على تقاطع جداول عمل تقويمين.

```csharp
public static ICalendar GetIntersectionCalendar(Calendar calendar1, Calendar calendar2)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| calendar1 | Calendar | التقويم الأول. |
| calendar2 | Calendar | التقويم الثاني. |

### قيمة الإرجاع

تنفيذ واجهة ICalendar.

### استثناءات

| استثناء | شرط |
| --- | --- |
| ArgumentNullException | عند كون أي من الوسائط فارغًا. |

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

* interface [ICalendar](../../icalendar/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


