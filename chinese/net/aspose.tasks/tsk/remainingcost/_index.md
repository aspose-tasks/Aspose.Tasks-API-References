---
title: "Tsk.RemainingCost"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。完成剩余计划工作时将产生的剩余计划费用"
type: docs
weight: 950
url: /zh/net/aspose.tasks/tsk/remainingcost/
---
## Tsk.RemainingCost field

完成剩余计划工作将产生的剩余计划费用。

```csharp
public static readonly Key<decimal, TaskKey> RemainingCost;
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


