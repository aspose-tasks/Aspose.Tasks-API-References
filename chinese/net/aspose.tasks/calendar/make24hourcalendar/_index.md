---
title: "Calendar.Make24HourCalendar"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Calendar 方法。将给定的 Calendar 设置为 24 小时日历。24 小时日历是指每周的每一天都以全天候工作时间运行的日历。"
type: docs
weight: 10
url: /zh/net/aspose.tasks/calendar/make24hourcalendar/
---
## Calendar.Make24HourCalendar method

将给定的 Calendar 设置为 24 小时日历。24 小时日历是一种日历，其中一周的每一天都以全天候工作时间运行。

```csharp
public static Calendar Make24HourCalendar(Calendar calendar)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 日历 | 日历 | 用于制作 24 小时日历的 Calendar。 |

### 返回值

24 小时日历。

## 示例

展示如何创建 24 小时日历。

```csharp
Project project = new Project();
var calendar = project.Calendars.Add("New calendar");
Calendar.Make24HourCalendar(calendar);

var workingHours = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0));

// 将打印 24 小时。
Console.WriteLine("Hours: " + workingHours.TotalHours);
```

展示如何将新日历转换为 24 小时日历。

```csharp
var project = new Project();

var calendar = project.Calendars.Add("24 Hours");
calendar = Calendar.Make24HourCalendar(calendar);

var workingHours = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0));

// 将打印 24 小时。
Console.WriteLine("Hours: " + workingHours.TotalHours);
```

### 另见

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


