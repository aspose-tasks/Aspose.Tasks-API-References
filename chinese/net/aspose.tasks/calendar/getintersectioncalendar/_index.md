---
title: "Calendar.GetIntersectionCalendar"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Calendar 方法。获取 ICalendar 实例，可用于对两个日历的工作计划交集进行计算"
type: docs
weight: 280
url: /zh/net/aspose.tasks/calendar/getintersectioncalendar/
---
## Calendar.GetIntersectionCalendar method

获取 [`ICalendar`](../../icalendar/) 实例，可用于对两个日历的工作计划交集进行计算。

```csharp
public static ICalendar GetIntersectionCalendar(Calendar calendar1, Calendar calendar2)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| calendar1 | 日历 | 第一个日历。 |
| calendar2 | 日历 | 第二个日历。 |

### 返回值

ICalendar 接口的实现。

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException | 当任意参数为 null 时。 |

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

* interface [ICalendar](../../icalendar/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


