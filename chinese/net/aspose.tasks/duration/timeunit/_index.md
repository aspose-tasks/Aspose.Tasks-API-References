---
title: "Duration.TimeUnit"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Duration 属性。获取此对象的时间单位类型。此 Duration 实例的时间单位类型。"
type: docs
weight: 50
url: /zh/net/aspose.tasks/duration/timeunit/
---
## Duration.TimeUnit property

获取此对象的时间单位类型。此 Duration 实例的时间单位类型。

```csharp
public TimeUnitType TimeUnit { get; }
```

## 示例

展示如何更新任务的持续时间。

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// 获取一个任务
var task1 = project.RootTask.Children.GetById(1);

// 更新任务的持续时间
var duration1 = task1.Get(Tsk.Duration);

// 为任务 1 添加一天
duration1 = duration1.Add(project.GetDuration(1, TimeUnitType.Day));

// 为任务设置新的持续时间
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// 获取另一个任务
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// 通过使用实际的时间单位类型更改持续时间
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Add(1d /* the time unit type of duration2 will be used */);

// 为任务设置新的持续时间
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task1.Get(Tsk.Duration));
```

### 另见

* enum [TimeUnitType](../../timeunittype/)
* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


