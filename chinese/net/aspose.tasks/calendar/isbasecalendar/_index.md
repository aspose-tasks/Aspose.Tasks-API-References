---
title: "Calendar.IsBaseCalendar"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Calendar 属性。获取指示日历是否为基础日历的值"
type: docs
weight: 70
url: /zh/net/aspose.tasks/calendar/isbasecalendar/
---
## Calendar.IsBaseCalendar property

获取一个值，指示该日历是否为基础日历。

```csharp
public bool IsBaseCalendar { get; }
```

## 示例

展示如何读取项目日历及其属性。

```csharp
var project = new Project(DataDir + "Project_GeneralCalendarProperties.xml");

foreach (var calendar in project.Calendars)
{
    if (calendar.Name == null)
    {
        continue;
    }

    Console.WriteLine("UID : " + calendar.Uid + " Name: " + calendar.Name);

    // 显示是否具有基础日历。
    Console.Write("Base Calendar : ");
    Console.WriteLine(calendar.IsBaseCalendar ? "Self" : calendar.BaseCalendar.Name);

    // 获取每个工作日的小时数。
    foreach (var wd in calendar.WeekDays)
    {
        var ts = wd.GetWorkingTime();
        Console.WriteLine("Day Type: " + wd.DayType + " Hours: " + ts);
    }
}
```

### 另见

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


