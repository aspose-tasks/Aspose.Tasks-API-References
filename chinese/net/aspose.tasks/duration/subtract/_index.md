---
title: "Duration.Subtract"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Duration 方法。从此持续时间实例中减去指定的持续时间。"
type: docs
weight: 100
url: /zh/net/aspose.tasks/duration/subtract/
---
## Subtract(Duration) {#subtract}

从此持续时间实例中减去指定的持续时间。

```csharp
public Duration Subtract(Duration d)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| d | Duration | 用于从此实例中减去的指定 [`Duration`](../) 实例。 |

### 返回值

表示此实例的值减去指定持续时间值的新 Duration 对象。

## 示例

展示如何更改任务的持续时间。

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// 获取一个任务
var task1 = project.RootTask.Children.GetById(1);

// 更新任务的持续时间
var duration1 = task1.Get(Tsk.Duration);

// 将任务 1 的持续时间减去一天。
duration1 = duration1.Subtract(project.GetDuration(1, TimeUnitType.Day));

// 为任务设置新的持续时间
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// 获取另一个任务
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// 通过使用实际的时间单位类型更改持续时间
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Subtract(1d /* the time unit type of duration2 will be used */);

// 为任务设置新的持续时间
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task2.Get(Tsk.Duration));
```

### 另见

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)

---

## Subtract(double) {#subtract_1}

从此持续时间实例中减去指定的 double 值。

```csharp
public Duration Subtract(double val)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| val | Double | 用于从此实例中减去的指定 Double 值。 |

### 返回值

表示此实例的值减去指定持续时间值的新 Duration 对象。

## 示例

展示如何更改任务的持续时间。

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// 获取一个任务
var task1 = project.RootTask.Children.GetById(1);

// 更新任务的持续时间
var duration1 = task1.Get(Tsk.Duration);

// 将任务 1 的持续时间减去一天。
duration1 = duration1.Subtract(project.GetDuration(1, TimeUnitType.Day));

// 为任务设置新的持续时间
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// 获取另一个任务
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// 通过使用实际的时间单位类型更改持续时间
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Subtract(1d /* the time unit type of duration2 will be used */);

// 为任务设置新的持续时间
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task2.Get(Tsk.Duration));
```

### 另见

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


