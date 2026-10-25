---
title: "Tsk.OvertimeCost"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。资源在所有分配任务或资源分配上的任务加班总成本"
type: docs
weight: 860
url: /zh/net/aspose.tasks/tsk/overtimecost/
---
## Tsk.OvertimeCost field

任务的加班总费用，或资源在所有分配任务上的加班费用，或资源分配的加班费用。

```csharp
public static readonly Key<decimal, TaskKey> OvertimeCost;
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
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


