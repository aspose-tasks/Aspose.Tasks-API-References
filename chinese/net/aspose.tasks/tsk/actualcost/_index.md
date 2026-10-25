---
title: "Tsk.ActualCost"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。资源在其任务上已完成工作产生的费用以及与任务相关的其他记录费用"
type: docs
weight: 20
url: /zh/net/aspose.tasks/tsk/actualcost/
---
## Tsk.ActualCost field

已由资源在其任务上完成的工作产生的成本，以及与任务相关的任何其他记录成本。

```csharp
public static readonly Key<decimal, TaskKey> ActualCost;
```

## 示例

展示如何读取任务的实际属性。

```csharp
var project = new Project(DataDir + "ActualTaskProperties.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// 遍历所有收集的任务
foreach (var task in collector.Tasks)
{
    Console.WriteLine("Task Name : " + task.Get(Tsk.Name));
    Console.WriteLine("Actual Start: " + task.Get(Tsk.ActualStart).ToLongDateString());
    Console.WriteLine("Actual Finish: " + task.Get(Tsk.ActualFinish).ToLongDateString());
    Console.WriteLine("Actual Duration: " + task.Get(Tsk.ActualDuration).TimeSpan.Hours);
    Console.WriteLine("Actual Cost: " + task.Get(Tsk.ActualCost));
}
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


