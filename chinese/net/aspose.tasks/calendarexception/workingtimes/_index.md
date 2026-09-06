---
title: "CalendarException.WorkingTimes"
second_title: "Aspose.Tasks for .NET API 参考"
description: "CalendarException 属性。获取或设置 WorkingTimeCollection 对象。该集合包含定义工作日工作时间的工作时间。至少必须存在一个工作时间，且不能超过五个。"
type: docs
weight: 160
url: /zh/net/aspose.tasks/calendarexception/workingtimes/
---
## CalendarException.WorkingTimes property

获取或设置 WorkingTimeCollection 对象。该集合定义了工作日的工作时间。必须至少存在一个工作时间，且不能超过五个。

```csharp
public WorkingTimeCollection WorkingTimes { get; set; }
```

## 示例

展示如何获取日历异常的工作时间。

```csharp
var project = new Project(DataDir + "CalendarExceptions.mpp");

var calendar = project.Calendars.ToList()[0];
var exception = calendar.Exceptions[0];

Console.WriteLine("Calendar Name: " + calendar.Name);
Console.WriteLine("Calendar Exception Count: " + calendar.Exceptions.Count);
Console.WriteLine("Calendar Exception Name: " + exception.Name);
Console.WriteLine();

var workingTime = exception.GetWorkingTime();
Console.WriteLine("Exception Working Time: " + workingTime);

foreach (var time in exception.WorkingTimes)
{
    Console.WriteLine("Working Time Start: " + time.From);
    Console.WriteLine("Working Time Finish: " + time.To);
}
```

### 另见

* class [WorkingTimeCollection](../../workingtimecollection/)
* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


