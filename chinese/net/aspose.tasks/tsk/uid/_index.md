---
title: "Tsk.Uid"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。任务的唯一标识符。"
type: docs
weight: 1110
url: /zh/net/aspose.tasks/tsk/uid/
---
## Tsk.Uid field

任务的唯一标识。

```csharp
public static readonly Key<int, TaskKey> Uid;
```

## 示例

展示如何读取/写入任务属性。

```csharp
var project = new Project();

// 添加任务并设置任务属性
var task = project.RootTask.Children.Add();
task.Set(Tsk.Name, "Task1");
task.Set(Tsk.Start, new DateTime(2020, 3, 31, 8, 0, 0));
task.Set(Tsk.Finish, new DateTime(2020, 3, 31, 17, 0, 0));

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// 遍历所有收集的任务
foreach (var tsk in collector.Tasks)
{
    Console.WriteLine("Task Id: {0}", tsk.Get(Tsk.Id));
    Console.WriteLine("Task Uid: {0}", tsk.Get(Tsk.Uid));
    Console.WriteLine("Task Name: {0}", tsk.Get(Tsk.Name));
    Console.WriteLine("Task Start: {0}", tsk.Get(Tsk.Start));
    Console.WriteLine("Task Finish: {0}", tsk.Get(Tsk.Finish));
}
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


