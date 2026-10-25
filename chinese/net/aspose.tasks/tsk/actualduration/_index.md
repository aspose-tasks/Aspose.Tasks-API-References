---
title: "Tsk.ActualDuration"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。基于计划持续时间和当前剩余工作量或完成百分比的任务实际工作时间跨度"
type: docs
weight: 30
url: /zh/net/aspose.tasks/tsk/actualduration/
---
## Tsk.ActualDuration field

基于计划持续时间和当前剩余工作或完成百分比的任务实际工作时间跨度。

```csharp
public static readonly Key<Duration, TaskKey> ActualDuration;
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
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


