---
title: "WorkUnit.From"
second_title: "Aspose.Tasks for .NET API 参考"
description: "WorkUnit 属性。获取或设置 From 日期"
type: docs
weight: 20
url: /zh/net/aspose.tasks/workunit/from/
---
## WorkUnit.From property

获取或设置 From 日期。

```csharp
public DateTime From { get; set; }
```

## 示例

展示如何使用工作单元信息。

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// 获取特定日期的工作时间
var workUnit = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0), new DateTime(2020, 4, 9, 17, 0, 0));

Console.WriteLine("From: " + workUnit.From);
Console.WriteLine("To: " + workUnit.To);
Console.WriteLine("Working hours: " + workUnit.WorkingHours);
```

### 另见

* class [WorkUnit](../)
* namespace [Aspose.Tasks](../../workunit/)
* assembly [Aspose.Tasks](../../../)


