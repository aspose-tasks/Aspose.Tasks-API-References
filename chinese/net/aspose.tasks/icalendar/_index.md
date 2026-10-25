---
title: "接口 ICalendar"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.ICalendar 接口。表示一种日历抽象，可用于各种日期和持续时间的计算。"
type: docs
weight: 840
url: /zh/net/aspose.tasks/icalendar/
---
## ICalendar interface

表示日历抽象，可用于各种日期和持续时间的计算。

```csharp
public interface ICalendar
```

## 方法

| 名称 | 描述 |
| --- | --- |
| [GetFinishDateByStartAndWork](../../aspose.tasks/icalendar/getfinishdatebystartandwork/#getfinishdatebystartandwork)(DateTime, Duration) | 根据日历计算指定工作时间量过去后的日期。 |
| [GetFinishDateByStartAndWork](../../aspose.tasks/icalendar/getfinishdatebystartandwork/#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | 根据日历计算指定工作时间量过去后的日期。 |
| [GetNextWorkingDayStart](../../aspose.tasks/icalendar/getnextworkingdaystart/)(DateTime) | 计算指定日期的下一个工作日开始时间。 |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/icalendar/getpreviousworkingdayend/)(DateTime) | 计算指定日期之前的工作日结束时间。 |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/icalendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration)(DateTime, Duration) | 根据指定的结束日期和持续时间返回开始日期。 |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/icalendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | 根据指定的结束日期和持续时间返回开始日期。 |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/icalendar/gettaskfinishdatefromduration/)(Task, TimeSpan) | 根据任务的开始日期、拆分部分和工作持续时间计算任务的完成日期和时间。 |
| [GetWorkingHours](../../aspose.tasks/icalendar/getworkinghours/#getworkinghours_1)(DateTime) | 返回指定日期的工作小时数。 |
| [GetWorkingHours](../../aspose.tasks/icalendar/getworkinghours/#getworkinghours)(DateTime, DateTime) | 返回 WorkUnit——指定日期时间间隔的工作小时的开始、结束和持续时间。 |
| [GetWorkingHoursTimeSpan](../../aspose.tasks/icalendar/getworkinghourstimespan/)(DateTime, DateTime) | 返回指定日期之间的工作小时数。 |
| [GetWorkingTimes](../../aspose.tasks/icalendar/getworkingtimes/)(DateTime) | 返回指定日期的工作时间的 [`WorkingTimeCollection`](../workingtimecollection/)。 |
| [GetWorkStart](../../aspose.tasks/icalendar/getworkstart/)(DateTime) | 计算从指定日期和时间开始的下一个工作时间的开始。 |
| [IsDayWorking](../../aspose.tasks/icalendar/isdayworking/)(DateTime) | 确定指定日期是否为日历中的工作日。 |
| [IsEmpty](../../aspose.tasks/icalendar/isempty/)() | 返回日历是否未定义工作时间。 |

## 示例

展示如何使用 Calendar.GetIntersectionCalendar() 方法在分配的日历上执行计算。

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

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


