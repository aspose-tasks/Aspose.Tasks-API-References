---
title: "Project.Calendars"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Project 属性。获取此 Project 实例的 CalendarCollection 对象。"
type: docs
weight: 130
url: /zh/net/aspose.tasks/project/calendars/
---
## Project.Calendars property

获取 [`CalendarCollection`](../../calendarcollection/) 对象，此 Project 实例。

```csharp
public CalendarCollection Calendars { get; }
```

## 示例

展示如何读取项目日历。

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

* class [CalendarCollection](../../calendarcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


