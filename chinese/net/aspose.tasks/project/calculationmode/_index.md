---
title: "Project.CalculationMode"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Project 属性。获取或设置项目的计算模式。可以是 CalculationMode 枚举的其中一个值"
type: docs
weight: 110
url: /zh/net/aspose.tasks/project/calculationmode/
---
## Project.CalculationMode property

获取或设置项目的计算模式。可以是 `CalculationMode` 枚举的其中一个值。

```csharp
public CalculationMode CalculationMode { get; set; }
```

## 示例

展示如何使用项目计算模式。

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

* enum [CalculationMode](../../calculationmode/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


