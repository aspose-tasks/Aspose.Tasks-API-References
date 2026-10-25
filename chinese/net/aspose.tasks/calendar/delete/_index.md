---
title: "Calendar.Delete"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Calendar 方法。从项目中删除日历"
type: docs
weight: 140
url: /zh/net/aspose.tasks/calendar/delete/
---
## Calendar.Delete method

从项目中移除日历。

```csharp
public void Delete()
```

## 示例

展示如何从项目中删除日历。

```csharp
var project = new Project(DataDir + "BrokenCalendar.mpp");

// 按名称获取日历
var calendar = project.Calendars.GetByName("Broken Calendar");

// 删除日历
calendar.Delete();
```

### 另见

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


