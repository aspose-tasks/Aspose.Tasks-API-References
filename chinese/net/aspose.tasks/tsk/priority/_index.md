---
title: "Tsk.Priority"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。任务的重要性级别，进而指示在资源平衡期间任务或分配被延迟或拆分的可能性。"
type: docs
weight: 930
url: /zh/net/aspose.tasks/tsk/priority/
---
## Tsk.Priority field

任务的重要性级别，这反映了在资源平衡期间任务或分配被延迟或拆分的可能性。

```csharp
public static readonly Key<int, TaskKey> Priority;
```

## 示例

展示如何读取任务优先级。

```csharp
var project = new Project(DataDir + "TaskPriority.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// 显示所有任务的优先级
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name) + " - Priority : " + task.Get(Tsk.Priority));
}
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


