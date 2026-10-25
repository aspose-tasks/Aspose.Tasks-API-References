---
title: "枚举 CalculationMode"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.CalculationMode 枚举。指定项目计算模式"
type: docs
weight: 210
url: /zh/net/aspose.tasks/calculationmode/
---
## CalculationMode enumeration

指定项目计算模式。

```csharp
public enum CalculationMode
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| None | `0` | 无。此模式下项目日期和成本不重新计算。 |
| Automatic | `1` | 自动模式。使用此模式时项目日期和成本会重新计算。 |
| Manual | `2` | 手动模式。此模式下仅重新计算必要字段，例如对象的 UID 和 ID。 |

## 示例

展示如何使用自动计算模式。

```csharp
var project = new Project
{
    CalculationMode = CalculationMode.Automatic
};

// 设置项目开始日期并添加新任务
project.Set(Prj.StartDate, new DateTime(2015, 4, 15));
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");

// 链接任务
project.TaskLinks.Add(task1, task2, TaskLinkType.FinishToStart);

// 验证日期已重新计算
Console.WriteLine("Task1 Start + 1 Equals Task2 Start : {0} ", task1.Get(Tsk.Start).AddDays(1).Equals(task2.Get(Tsk.Start)));
Console.WriteLine("Task1 Finish + 1 Equals Task2 Finish : {0} ", task1.Get(Tsk.Finish).AddDays(1).Equals(task2.Get(Tsk.Finish)));
Console.WriteLine("RootTask Finish Equals Task2 Finish : {0} ", task2.Get(Tsk.Finish).Equals(project.RootTask.Get(Tsk.Finish)));
Console.WriteLine("Project Finish Date Equals Task2 Finish : {0} ", task2.Get(Tsk.Finish).Equals(project.Get(Prj.FinishDate)));
```

展示如何使用无计算模式。

```csharp
var project = new Project
{
    CalculationMode = CalculationMode.None
};

// 添加新任务
var task = project.RootTask.Children.Add("Task");

// 注意，即使 ID 也未被计算
Console.WriteLine("Task.Id Equals 0 : {0} ", task.Get(Tsk.Id).Equals(0));
Console.WriteLine("Task.OutlineLevel Equals 0 : {0} ", task.Get(Tsk.OutlineLevel).Equals(0));
Console.WriteLine("Task Start Equals DateTime.MinValue : {0} ", task.Get(Tsk.Start).Equals(DateTime.MinValue));
Console.WriteLine("Task Finish Equals DateTime.MinValue : {0} ", task.Get(Tsk.Finish).Equals(DateTime.MinValue));
Console.WriteLine("Task Duration Equals 0 mins : {0} ", task.Get(Tsk.Duration).ToString().Equals("0 mins"));

// 设置 duration 属性
task.Set(Tsk.Duration, project.GetDuration(2, TimeUnitType.Day));
Console.WriteLine("Task Duration Equals 2 days : {0} ", task.Get(Tsk.Duration).ToString().Equals("2 days"));
Console.WriteLine("Task Start Equals DateTime.MinValue  : {0} ", task.Get(Tsk.Start).Equals(DateTime.MinValue));
Console.WriteLine("Task Finish Equals DateTime.MinValue  : {0} ", task.Get(Tsk.Finish).Equals(DateTime.MinValue));
```

展示如何使用手动计算模式。

```csharp
var project = new Project
{
    CalculationMode = CalculationMode.Manual
};

// 设置项目开始日期并添加新任务
project.Set(Prj.StartDate, new DateTime(2015, 4, 15));
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");

// 必要的属性已在手动模式中设置
Console.WriteLine("Task1.Id Equals 1 : {0} ", task1.Get(Tsk.Id).Equals(1));
Console.WriteLine("Task1 OutlineLevel Equals 1 : {0} ", task1.Get(Tsk.OutlineLevel).Equals(1));
Console.WriteLine("Task1 Start Equals 15/04/2015 08:00 AM : {0} ", task1.Get(Tsk.Start).Equals(new DateTime(2015, 4, 15, 8, 0, 0)));
Console.WriteLine("Task1 Finish Equals 15/04/2015 05:00 PM : {0} ", task1.Get(Tsk.Finish).Equals(new DateTime(2015, 4, 15, 17, 0, 0)));
Console.WriteLine("Task1 Duration Equals 1 day : {0} ", task1.Get(Tsk.Duration).ToString().Equals("1 day"));
Console.WriteLine("Task2 Start Equals 15/04/2015 08:00 AM : {0} ", task2.Get(Tsk.Start).Equals(new DateTime(2015, 4, 15, 8, 0, 0)));
Console.WriteLine("Task2 Finish Equals 15/04/2015 05:00 PM : {0} ", task2.Get(Tsk.Finish).Equals(new DateTime(2015, 4, 15, 17, 0, 0)));
Console.WriteLine("Task2 Duration Equals 1 day : {0} ", task2.Get(Tsk.Duration).ToString().Equals("1 day"));

// 当我们将两个任务链接在一起时，它们的日期在手动模式下不会重新计算
project.TaskLinks.Add(task1, task2, TaskLinkType.FinishToStart);

// 任务 2 的开始时间未被更改
Console.WriteLine("Task1 Start Equals Task2 Start : {0} ", task1.Get(Tsk.Start).Equals(task2.Get(Tsk.Start)));
Console.WriteLine("Task1 Finish Equals Task2 Finish : {0} ", task1.Get(Tsk.Finish).Equals(task2.Get(Tsk.Finish)));
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


