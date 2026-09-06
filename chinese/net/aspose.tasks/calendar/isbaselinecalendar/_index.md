---
title: "Calendar.IsBaselineCalendar"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Calendar 属性。获取或设置指示日历是否为基线日历的值"
type: docs
weight: 80
url: /zh/net/aspose.tasks/calendar/isbaselinecalendar/
---
## Calendar.IsBaselineCalendar property

获取或设置一个值，指示该日历是否为基线日历。

```csharp
public bool IsBaselineCalendar { get; set; }
```

## 示例

展示如何检查日历是否为基线日历。

```csharp
var project = new Project(DataDir + "IsBaselineCalendar.mpp");

var calendar = project.Calendars.GetByUid(3);

Console.WriteLine("Is baseline calendar: " + calendar.IsBaselineCalendar);
```

### 另见

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


