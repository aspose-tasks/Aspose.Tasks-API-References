---
title: "Tsk.OutlineNumber"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。表示任务在层次大纲结构中位置的编号"
type: docs
weight: 850
url: /zh/net/aspose.tasks/tsk/outlinenumber/
---
## Tsk.OutlineNumber field

表示任务在层次大纲结构中位置的编号。

```csharp
public static readonly Key<string, TaskKey> OutlineNumber;
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


