---
title: "Tsk.OvertimeWork"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk field. 所有分配给任务的资源计划执行的加班工作量."
type: docs
weight: 870
url: /zh/net/aspose.tasks/tsk/overtimework/
---
## Tsk.OvertimeWork field

分配给任务的所有资源计划执行的加班量。

```csharp
public static readonly Key<Duration, TaskKey> OvertimeWork;
```

## 示例

展示如何读取任务加班情况。

```csharp
var project = new Project(DataDir + "TaskOvertimes.mpp");

// 读取任务的加班和完成百分比
foreach (var task in project.RootTask.Children)
{
    Console.WriteLine(task.Get(Tsk.OvertimeCost));
    Console.WriteLine(task.Get(Tsk.OvertimeWork));
    Console.WriteLine(task.Get(Tsk.PercentComplete));
    Console.WriteLine(task.Get(Tsk.PercentWorkComplete));
    Console.WriteLine(task.Get(Tsk.PhysicalPercentComplete));

    // 设置完成百分比
    task.Set(Tsk.PercentComplete, 100);
}
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


