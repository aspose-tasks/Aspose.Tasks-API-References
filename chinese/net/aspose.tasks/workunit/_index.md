---
title: "类 WorkUnit"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.WorkUnit 类。表示工作时间"
type: docs
weight: 3630
url: /zh/net/aspose.tasks/workunit/
---
## WorkUnit class

表示工作时间。

```csharp
public class WorkUnit
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [WorkUnit](workunit/)(DateTime, DateTime) | 初始化 `WorkUnit` 类的新实例。使用指定的 From 和 To 日期创建新的 WorkUnit 对象。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [From](../../aspose.tasks/workunit/from/) { get; set; } | 获取或设置 From 日期。 |
| [To](../../aspose.tasks/workunit/to/) { get; set; } | 获取或设置 To 日期。 |
| [WorkingHours](../../aspose.tasks/workunit/workinghours/) { get; set; } | 获取或设置工作时间的持续时间。 |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


