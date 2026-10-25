---
title: "Tsk.IsEstimated"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。确定任务是否为估算任务"
type: docs
weight: 580
url: /zh/net/aspose.tasks/tsk/isestimated/
---
## Tsk.IsEstimated field

确定任务是否为估计任务。

```csharp
public static readonly Key<NullableBool, TaskKey> IsEstimated;
```

## 示例

展示如何查找估计任务和/或里程碑任务。

```csharp
var prj = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(prj.RootTask, collector, 0);

// 遍历收集的任务
foreach (var task in collector.Tasks)
{
    var estimated = task.Get(Tsk.IsEstimated).Value ? "Estimated" : "Non-Estimated";
    var milestone = task.Get(Tsk.IsMilestone).Value ? "Milestone" : "Non-Milestone";
    Console.WriteLine(task.Get(Tsk.Name) + " : " + estimated);
    Console.WriteLine(task.Get(Tsk.Name) + " : " + milestone);
}
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


