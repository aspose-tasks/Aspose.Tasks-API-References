---
title: "Prj.Calendar"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。项目日历"
type: docs
weight: 90
url: /zh/net/aspose.tasks/prj/calendar/
---
## Prj.Calendar field

项目日历。

```csharp
public static readonly Key<Calendar, PrjKey> Calendar;
```

## 示例

展示如何读取/写入 Prj.Calendar 属性。

```csharp
var project = new Project();
var calendar = project.Calendars.Add("Standard");
Calendar.MakeStandardCalendar(calendar);

project.Set(Prj.Calendar, calendar);

Console.WriteLine("Calendar: " + project.Get(Prj.Calendar).Name);
foreach (var weekDay in calendar.WeekDays)
{
    Console.WriteLine(weekDay.FromDate);
    Console.WriteLine(weekDay.ToDate);
}
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Calendar](../../calendar/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


