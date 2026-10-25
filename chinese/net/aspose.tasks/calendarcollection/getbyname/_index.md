---
title: "CalendarCollection.GetByName"
second_title: "Aspose.Tasks for .NET API 参考"
description: "CalendarCollection 方法。返回具有指定名称的日历"
type: docs
weight: 30
url: /zh/net/aspose.tasks/calendarcollection/getbyname/
---
## CalendarCollection.GetByName method

返回具有指定名称的日历。

```csharp
public Calendar GetByName(string name)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 名称 | 字符串 | 日历的名称。 |

### 返回值

如果找到，则返回具有指定名称的日历；否则返回 null。

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


