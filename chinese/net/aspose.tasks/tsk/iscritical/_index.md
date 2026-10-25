---
title: "Tsk.IsCritical"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。确定任务是否位于关键路径上。"
type: docs
weight: 560
url: /zh/net/aspose.tasks/tsk/iscritical/
---
## Tsk.IsCritical field

确定任务是否位于关键路径上。

```csharp
public static readonly Key<NullableBool, TaskKey> IsCritical;
```

## 示例

展示如何查找关键任务和/或努力驱动任务。

```csharp
var project = new Project(DataDir + "CriticalEffortDrivenTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// 遍历所有收集的任务
foreach (var task in collector.Tasks)
{
    var effortDriven = task.Get(Tsk.IsEffortDriven).Value ? "EffortDriven" : "Non-EffortDriven";
    var nonCritical = task.Get(Tsk.IsCritical).Value ? "Critical" : "Non-Critical";
    Console.WriteLine(task.Get(Tsk.Name) + " : " + effortDriven);
    Console.WriteLine(task.Get(Tsk.Name) + " : " + nonCritical);
}
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


