---
title: "Task.Predecessors"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Task 属性。获取一个 TaskCollection 对象，其中包含此 Task 对象的所有前置任务"
type: docs
weight: 980
url: /zh/net/aspose.tasks/task/predecessors/
---
## Task.Predecessors property

获取一个 [`TaskCollection`](../../taskcollection/) 对象，其中包含此 Task 对象的所有前置任务。

```csharp
public TaskCollection Predecessors { get; }
```

### 返回值

只读的 [`TaskCollection`](../../taskcollection/) 类实例。

## 示例

展示如何读取任务的前置任务。

```csharp
var project = new Project();
var pred = project.RootTask.Children.Add("Predecessor");
var succ = project.RootTask.Children.Add("Successor");

project.TaskLinks.Add(pred, succ);

foreach (var predecessor in succ.Predecessors)
{
    Console.WriteLine("{0} {1}", predecessor.Get(Tsk.Id), predecessor.Get(Tsk.Name));
}
```

### 另见

* class [TaskCollection](../../taskcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


