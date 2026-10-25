---
title: "الواجهة ICalendar"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "واجهة Aspose.Tasks.ICalendar. تمثل تجريدًا للتقويم يمكن استخدامه لمختلف حسابات التواريخ والمدة."
type: docs
weight: 840
url: /ar/net/aspose.tasks/icalendar/
---
## ICalendar interface

يمثل تجريدًا للتقويم يمكن استخدامه في حسابات مختلفة للتواريخ والمدة.

```csharp
public interface ICalendar
```

## الطرق

| الاسم | الوصف |
| --- | --- |
| [GetFinishDateByStartAndWork](../../aspose.tasks/icalendar/getfinishdatebystartandwork/#getfinishdatebystartandwork)(DateTime, Duration) | يحسب التاريخ الذي سينقضي فيه مقدار وقت العمل المحدد وفقًا للتقويم. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/icalendar/getfinishdatebystartandwork/#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | يحسب التاريخ الذي سينقضي فيه مقدار وقت العمل المحدد وفقًا للتقويم. |
| [GetNextWorkingDayStart](../../aspose.tasks/icalendar/getnextworkingdaystart/)(DateTime) | يحسب بداية يوم العمل التالي للتاريخ المحدد. |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/icalendar/getpreviousworkingdayend/)(DateTime) | يحسب نهاية تاريخ العمل السابق من التاريخ المحدد. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/icalendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration)(DateTime, Duration) | يرجع تاريخ البدء بناءً على تاريخ الانتهاء المحدد والمدة. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/icalendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | يرجع تاريخ البدء بناءً على تاريخ الانتهاء المحدد والمدة. |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/icalendar/gettaskfinishdatefromduration/)(Task, TimeSpan) | يحسب تاريخ ووقت انتهاء المهمة من تاريخ بدايتها، الأجزاء المقسمة ومدة العمل. |
| [GetWorkingHours](../../aspose.tasks/icalendar/getworkinghours/#getworkinghours_1)(DateTime) | يرجع مقدار ساعات العمل في التاريخ المحدد. |
| [GetWorkingHours](../../aspose.tasks/icalendar/getworkinghours/#getworkinghours)(DateTime, DateTime) | يرجع WorkUnit - بداية، انتهاء ومدة ساعات العمل للفترة الزمنية المحددة. |
| [GetWorkingHoursTimeSpan](../../aspose.tasks/icalendar/getworkinghourstimespan/)(DateTime, DateTime) | يرجع مقدار ساعات العمل بين التواريخ المحددة. |
| [GetWorkingTimes](../../aspose.tasks/icalendar/getworkingtimes/)(DateTime) | يرجع [`WorkingTimeCollection`](../workingtimecollection/) لأوقات العمل للتاريخ المحدد. |
| [GetWorkStart](../../aspose.tasks/icalendar/getworkstart/)(DateTime) | يحسب بداية وقت العمل التالي بدءًا من التاريخ والوقت المحددين. |
| [IsDayWorking](../../aspose.tasks/icalendar/isdayworking/)(DateTime) | يحدد ما إذا كان اليوم المحدد يوم عمل وفقًا للتقويم. |
| [IsEmpty](../../aspose.tasks/icalendar/isempty/)() | يرجع ما إذا كان التقويم لا يحتوي على ساعات عمل معرفة. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


