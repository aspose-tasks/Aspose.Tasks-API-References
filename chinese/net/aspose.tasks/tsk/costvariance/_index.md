---
title: "Tsk.CostVariance"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。任务资源或分配的基线成本与总成本之间的差异。"
type: docs
weight: 240
url: /zh/net/aspose.tasks/tsk/costvariance/
---
## Tsk.CostVariance field

任务、资源或分配的基准成本与总成本之间的差额。

```csharp
public static readonly Key<double, TaskKey> CostVariance;
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


