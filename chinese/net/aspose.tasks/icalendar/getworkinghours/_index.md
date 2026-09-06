---
title: "ICalendar.GetWorkingHours"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ICalendar 方法。返回指定日期时间间隔的工作时间的 WorkUnit 开始、结束和持续时间。"
type: docs
weight: 60
url: /zh/net/aspose.tasks/icalendar/getworkinghours/
---
## GetWorkingHours(DateTime, DateTime) {#getworkinghours}

返回 WorkUnit——指定日期时间间隔的工作小时的开始、结束和持续时间。

```csharp
public WorkUnit GetWorkingHours(DateTime start, DateTime finish)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 开始 | DateTime | 区间的开始日期。 |
| 结束 | DateTime | 区间的结束日期。 |

### 返回值

[`WorkUnit`](../../workunit/) 类的实例，包含工作时间的开始、结束和持续时间。

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

* class [WorkUnit](../../workunit/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetWorkingHours(DateTime) {#getworkinghours_1}

返回指定日期的工作小时数。

```csharp
public TimeSpan GetWorkingHours(DateTime dt)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| dt | DateTime | 获取工作时间的日期。 |

### 返回值

指定日期的工作时间。

### 另见

* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


