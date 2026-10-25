---
title: "Tsk.OutlineLevel"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。任务的轮廓级别"
type: docs
weight: 840
url: /zh/net/aspose.tasks/tsk/outlinelevel/
---
## Tsk.OutlineLevel field

任务的大纲层级。

```csharp
public static readonly Key<int, TaskKey> OutlineLevel;
```

## 示例

展示如何读取任务轮廓属性。

```csharp
var project = new Project(DataDir + "TaskOutlineProperties.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// 遍历所有收集的任务
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name) + " - Outline Level : " + task.Get(Tsk.OutlineLevel));
    Console.WriteLine(task.Get(Tsk.Name) + " - Outline Number : " + task.Get(Tsk.OutlineNumber));
}
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


