---
title: "结构体 Duration"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Duration 结构体。表示项目中的持续时间。"
type: docs
weight: 470
url: /zh/net/aspose.tasks/duration/
---
## Duration structure

表示项目中的持续时间。

```csharp
public struct Duration : IEquatable<Duration>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [IsElapsed](../../aspose.tasks/duration/iselapsed/) { get; } | 获取一个值，指示时间单位是否已过去。此标志决定此 Duration 实例是否已过去。 |
| [IsEstimated](../../aspose.tasks/duration/isestimated/) { get; } | 获取一个值，指示时间单位是否为估计。此标志决定此 Duration 实例是否为估计。 |
| [TimeSpan](../../aspose.tasks/duration/timespan/) { get; } | 获取此 Duration 对象的 [`TimeSpan`](./timespan/) 实例。此 Duration 对象的 TimeSpan 实例。 |
| [TimeUnit](../../aspose.tasks/duration/timeunit/) { get; } | 获取此对象的时间单位类型。此 Duration 实例的时间单位类型。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| static [Parse](../../aspose.tasks/duration/parse/)(Project, string) | 将指定的字符串转换为 `Duration` 结构体的实例。 |
| [Add](../../aspose.tasks/duration/add/#add_1)(double) | 将指定的 double 值添加到此持续时间。 |
| [Add](../../aspose.tasks/duration/add/#add)(Duration) | 将指定的持续时间添加到此持续时间。 |
| [Convert](../../aspose.tasks/duration/convert/)(TimeUnitType) | 将 Duration 对象转换为具有指定时间单位的另一个持续时间。 |
| [Equals](../../aspose.tasks/duration/equals/#equals)(Duration) | 返回一个值，指示此实例是否等于指定的对象。 |
| override [Equals](../../aspose.tasks/duration/equals/#equals_1)(object) | 返回一个值，指示此实例是否等于指定的对象。 |
| override [GetHashCode](../../aspose.tasks/duration/gethashcode/)() | 返回此对象的哈希码值。 |
| [Subtract](../../aspose.tasks/duration/subtract/#subtract_1)(double) | 从此持续时间实例中减去指定的 double 值。 |
| [Subtract](../../aspose.tasks/duration/subtract/#subtract)(Duration) | 从此持续时间实例中减去指定的持续时间。 |
| [ToDouble](../../aspose.tasks/duration/todouble/)() | 将 Duration 对象转换为 Double 值。 |
| override [ToString](../../aspose.tasks/duration/tostring/)() | 返回此实例的字符串表示。 |
| static [ParseTimeSpan](../../aspose.tasks/duration/parsetimespan/)(string) | 解析格式为 "PT--H--M--S--" 的持续时间字符串。 |
| [operator ==](../../aspose.tasks/duration/op_equality/) | 返回一个值，指示此实例是否等于指定的对象。 |
| [operator !=](../../aspose.tasks/duration/op_inequality/) | 返回一个值，指示此实例是否不等于指定的对象。 |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


