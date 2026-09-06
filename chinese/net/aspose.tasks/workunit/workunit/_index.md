---
title: "WorkUnit.WorkUnit"
second_title: "Aspose.Tasks for .NET API 参考"
description: "WorkUnit 构造函数。初始化 WorkUnit 类的新实例。使用指定的 From 和 To 日期创建新的 WorkUnit 对象"
type: docs
weight: 10
url: /zh/net/aspose.tasks/workunit/workunit/
---
## WorkUnit constructor

初始化 [`WorkUnit`](../) 类的新实例。使用指定的 From 和 To 日期创建新的 WorkUnit 对象。

```csharp
public WorkUnit(DateTime from, DateTime to)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| from | DateTime | 工作时间的开始日期。 |
| 至 | DateTime | 工作时间的结束日期。 |

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


