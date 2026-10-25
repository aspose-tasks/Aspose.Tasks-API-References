---
title: "Tsk.WBSLevel"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。任务的最右侧 WBS 级别"
type: docs
weight: 1140
url: /zh/net/aspose.tasks/tsk/wbslevel/
---
## Tsk.WBSLevel field

任务最右侧的 WBS 级别。

```csharp
public static readonly Key<string, TaskKey> WBSLevel;
```

## 示例

展示如何读取任务的 WBS 代码。

```csharp
var project = new Project(DataDir + "TaskWBS.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// 遍历所有收集的任务
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.WBS));
    Console.WriteLine(task.Get(Tsk.WBSLevel));
}
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


