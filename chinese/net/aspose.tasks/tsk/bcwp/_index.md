---
title: "Tsk.BCWP"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。任务完成百分比乘以分阶段基线成本的累计值"
type: docs
weight: 120
url: /zh/net/aspose.tasks/tsk/bcwp/
---
## Tsk.BCWP field

任务完成百分比乘以时间分阶段基线成本的累计值。

```csharp
public static readonly Key<double, TaskKey> BCWP;
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


