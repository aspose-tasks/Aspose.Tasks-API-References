---
title: "Task.SelectAllChildTasks"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Task 方法。递归收集此任务的所有子任务"
type: docs
weight: 1400
url: /zh/net/aspose.tasks/task/selectallchildtasks/
---
## Task.SelectAllChildTasks method

递归收集此任务的所有子任务。

```csharp
public IEnumerable<Task> SelectAllChildTasks()
```

### 返回值

此任务的子任务列表。

## 示例

展示如何遍历子任务。

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task 1");
task.Children.Add("Task 2");

foreach (var tsk in project.RootTask.SelectAllChildTasks())
{
    Console.WriteLine("{0} {1}", tsk.Get(Tsk.Id), tsk.Get(Tsk.Name));
}
```

### 另见

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


