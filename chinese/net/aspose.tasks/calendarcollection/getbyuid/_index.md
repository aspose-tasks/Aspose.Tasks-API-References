---
title: "CalendarCollection.GetByUid"
second_title: "Aspose.Tasks for .NET API 参考"
description: "CalendarCollection 方法。返回具有指定 UID 的日历"
type: docs
weight: 40
url: /zh/net/aspose.tasks/calendarcollection/getbyuid/
---
## CalendarCollection.GetByUid method

返回具有指定 UID 的日历。

```csharp
public Calendar GetByUid(int uid)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| uid | Int32 | 日历的 UID。 |

### 返回值

具有指定 UID 的日历。

## 示例

展示如何按名称或按 ID 获取日历。

```csharp
var project = new Project(DataDir + "Project5.mpp");

var calendarByName = project.Calendars.GetByName("TestCalendar");
var calendarByUid = project.Calendars.GetByUid(4);

Console.WriteLine("Calendar Name: " + calendarByName.Name);
Console.WriteLine("Calendar Name: " + calendarByUid.Name);
Console.WriteLine("Are calendars equals: " + calendarByName.Equals(calendarByUid));
```

### 另见

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


