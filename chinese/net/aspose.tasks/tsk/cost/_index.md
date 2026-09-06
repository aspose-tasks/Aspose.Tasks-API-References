---
title: "Tsk.Cost"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk field. 基于已分配给任务的资源已完成工作产生的费用以及计划用于剩余工作的费用，对任务的总计划或预计成本进行说明."
type: docs
weight: 230
url: /zh/net/aspose.tasks/tsk/cost/
---
## Tsk.Cost field

任务的总计划或预计成本，基于已分配资源完成工作已产生的成本以及剩余工作计划的成本。

```csharp
public static readonly Key<decimal, TaskKey> Cost;
```

## 示例

展示如何读取任务成本。

```csharp
var project = new Project();

// 添加任务并设置成本
var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Cost, 800);

// 显示任务的成本相关属性
Console.WriteLine(task.Get(Tsk.RemainingCost));
Console.WriteLine(task.Get(Tsk.FixedCost));
Console.WriteLine(task.Get(Tsk.CostVariance));
Console.WriteLine(project.RootTask.Get(Tsk.Cost));
Console.WriteLine(project.RootTask.Get(Tsk.FixedCost));
Console.WriteLine(project.RootTask.Get(Tsk.RemainingCost));
Console.WriteLine(project.RootTask.Get(Tsk.CostVariance));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


