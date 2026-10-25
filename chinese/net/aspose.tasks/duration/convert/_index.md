---
title: "Duration.Convert"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Duration 方法。将 Duration 对象转换为具有指定时间单位的另一个持续时间。"
type: docs
weight: 70
url: /zh/net/aspose.tasks/duration/convert/
---
## Duration.Convert method

将 Duration 对象转换为具有指定时间单位的另一个持续时间。

```csharp
public Duration Convert(TimeUnitType timeUnitType)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| timeUnitType | TimeUnitType | 指定的时间单位类型。 |

### 返回值

返回具有指定单位类型的新 Duration。

## 示例

展示如何将持续时间转换为不同的时间单位类型。

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// 获取任务以计算其持续时间的不同格式
var task = project.RootTask.Children.GetById(1);

// 获取以分钟、天、小时、周和月为单位的持续时间
var mins = task.Get(Tsk.Duration).Convert(TimeUnitType.Minute).ToDouble();
Console.WriteLine("Duration in Mins: {0}", mins);
var days = task.Get(Tsk.Duration).Convert(TimeUnitType.Day).ToDouble();
Console.WriteLine("Duration in Days: {0}", days);
var hours = task.Get(Tsk.Duration).Convert(TimeUnitType.Hour).ToDouble();
Console.WriteLine("Duration in Hours: {0}", hours);
var weeks = task.Get(Tsk.Duration).Convert(TimeUnitType.Week).ToDouble();
Console.WriteLine("Duration in Weeks: {0}", weeks);
var months = task.Get(Tsk.Duration).Convert(TimeUnitType.Month).ToDouble();
Console.WriteLine("Duration in Months: {0}", months);
```

### 另见

* enum [TimeUnitType](../../timeunittype/)
* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


