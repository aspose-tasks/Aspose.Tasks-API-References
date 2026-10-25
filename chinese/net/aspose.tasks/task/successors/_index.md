---
title: "Task.Successors"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Task 属性。获取一个 TaskCollection 对象，其中包含此 Task 对象的所有后继任务"
type: docs
weight: 1200
url: /zh/net/aspose.tasks/task/successors/
---
## Task.Successors property

获取一个 [`TaskCollection`](../../taskcollection/) 对象，其中包含此 Task 对象的所有后继任务。

```csharp
public TaskCollection Successors { get; }
```

### 返回值

只读的 [`TaskCollection`](../../taskcollection/) 类实例。

## 示例

展示如何读取任务的后继。

```csharp
var project = new Project();
var pred = project.RootTask.Children.Add("Predecessor");
var succ = project.RootTask.Children.Add("Successor");

project.TaskLinks.Add(pred, succ);

foreach (var successor in pred.Successors)
{
    Console.WriteLine("{0} {1}", successor.Get(Tsk.Id), successor.Get(Tsk.Name));
}
```

### 另见

* class [TaskCollection](../../taskcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


