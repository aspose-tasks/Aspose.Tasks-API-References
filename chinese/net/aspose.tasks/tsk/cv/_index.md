---
title: "Tsk.CV"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。任务的基准成本与总成本之间的差额。成本差异  成本  基准成本"
type: docs
weight: 260
url: /zh/net/aspose.tasks/tsk/cv/
---
## Tsk.CV field

任务的基准成本与总成本之间的差额。成本差异 = 成本 - 基准成本。

```csharp
public static readonly Key<double, TaskKey> CV;
```

## 示例

展示如何读取任务成本值。

```csharp
var project = new Project(DataDir + "ResourceAssignmentCosts.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

foreach (var task in collector.Tasks)
{
    Console.WriteLine("Cost: " + task.Get(Tsk.Cost));
    Console.WriteLine("ACWP: " + task.Get(Tsk.ACWP));
    Console.WriteLine("BCWP: " + task.Get(Tsk.BCWP));
    Console.WriteLine("BCWS: " + task.Get(Tsk.BCWS));

    // CV = BCWP - ACWP
    Console.WriteLine("CV: " + task.Get(Tsk.CV));
    Console.WriteLine();
}
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


