---
title: "Duration.TimeSpan"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Duration 属性。获取此 Duration 对象的 TimeSpan 实例。此 Duration 对象的 TimeSpan 实例。"
type: docs
weight: 40
url: /zh/net/aspose.tasks/duration/timespan/
---
## Duration.TimeSpan property

获取此 Duration 对象的 `TimeSpan` 实例。此 Duration 对象的 TimeSpan 实例。

```csharp
public TimeSpan TimeSpan { get; }
```

## 示例

展示如何将持续时间转换为 TimeSpan。

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");
var task = project.RootTask.Children.GetById(1);

// 获取任务的 Duration。
var duration = task.Get(Tsk.Duration);
Console.WriteLine("Time span of duration: " + duration.TimeSpan);
```

### 另见

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


