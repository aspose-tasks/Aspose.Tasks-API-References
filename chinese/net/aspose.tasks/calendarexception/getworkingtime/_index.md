---
title: "CalendarException.GetWorkingTime"
second_title: "Aspose.Tasks for .NET API 参考"
description: "CalendarException 方法。返回日历异常的工作时间。"
type: docs
weight: 200
url: /zh/net/aspose.tasks/calendarexception/getworkingtime/
---
## CalendarException.GetWorkingTime method

返回日历例外的工作时间。

```csharp
public TimeSpan GetWorkingTime()
```

### 返回值

返回此日历异常的工作时间。

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

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


