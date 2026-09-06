---
title: "Calendar.PrimaveraProperties"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Calendar 属性。获取一个对象，该对象包含从 Primavera 格式读取的日历的 Primavera 特定属性。"
type: docs
weight: 100
url: /zh/net/aspose.tasks/calendar/primaveraproperties/
---
## Calendar.PrimaveraProperties property

获取一个对象，包含从 Primavera 格式读取的日历的 Primavera 特定属性。

```csharp
public PrimaveraCalendarProperties PrimaveraProperties { get; }
```

## 示例

展示如何从 Primavera 文件读取项目并检查日历的 Primavera 特定属性。

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 4861;

// 返回具有特殊 UID 的项目
var project = new Project(DataDir + "ScheduleOptions.xer", options);

var calendar = project.Calendars.GetByUid(178);

Console.WriteLine("Hours per day in '{0}' : {1}", calendar.Name, calendar.PrimaveraProperties.HoursPerDay);
```

### 另见

* class [PrimaveraCalendarProperties](../../primaveracalendarproperties/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


