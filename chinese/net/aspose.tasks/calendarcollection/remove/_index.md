---
title: "CalendarCollection.Remove"
second_title: "Aspose.Tasks for .NET API 参考"
description: "CalendarCollection 方法。将 Calendar 从 Project CalendarCollection 中移除"
type: docs
weight: 60
url: /zh/net/aspose.tasks/calendarcollection/remove/
---
## CalendarCollection.Remove method

从项目 CalendarCollection 中移除日历。

```csharp
public bool Remove(Calendar item)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| item | 日历 | 要移除的日历。 |

### 返回值

如果已移除则返回 true，否则返回 false。

### 异常

| 异常 | 条件 |
| --- | --- |
| InvalidOperationException | 当无法移除日历时抛出此异常。 |

## 示例

展示如何在集合中替换日历。

```csharp
var project = new Project(DataDir + "Project5.mpp");

var calendar = project.Calendars.GetByName("TestCalendar");
if (calendar != null)
{
    project.Calendars.Remove(calendar);
}

// 添加新日历
project.Calendars.Add("New Calendar");
project.Save(OutDir + "ReplaceCalendarWithNewCalendar_out.mpp", SaveFileFormat.Mpp);
```

### 另见

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


