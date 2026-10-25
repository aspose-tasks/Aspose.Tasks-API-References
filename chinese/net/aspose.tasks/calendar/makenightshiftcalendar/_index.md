---
title: "Calendar.MakeNightShiftCalendar"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Calendar 方法。将给定的 Calendar 设置为夜班日历"
type: docs
weight: 20
url: /zh/net/aspose.tasks/calendar/makenightshiftcalendar/
---
## Calendar.MakeNightShiftCalendar method

将给定的日历设为夜班日历。

```csharp
public static Calendar MakeNightShiftCalendar(Calendar calendar)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 日历 | 日历 | 用于创建夜班日历的 Calendar。 |

### 返回值

夜班日历。

## 示例

展示如何创建夜班日历。

```csharp
Project project = new Project();
var calendar = project.Calendars.Add("New calendar");
Calendar.MakeNightShiftCalendar(calendar);

var workingHours = calendar.GetWorkingTimes(new DateTime(2020, 4, 8));

// 显示工作时间
foreach (var wh in workingHours)
{
    Console.WriteLine("From: " + wh.From);
    Console.WriteLine("To: " + wh.To);
}
```

展示如何将日历转换为夜班日历。

```csharp
var project = new Project();

var calendar = project.Calendars.Add("Night Shift");
calendar = Calendar.MakeNightShiftCalendar(calendar);

var workingHours = calendar.GetWorkingTimes(new DateTime(2020, 4, 8));

// 显示工作时间
foreach (var wh in workingHours)
{
    Console.WriteLine("From: " + wh.From);
    Console.WriteLine("To: " + wh.To);
}
```

### 另见

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


