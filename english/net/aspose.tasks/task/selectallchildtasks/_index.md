---
title: Task.SelectAllChildTasks
second_title: Aspose.Tasks for .NET API Reference
description: Task method. Recursively collects all child tasks of this task
type: docs
weight: 1400
url: /net/aspose.tasks/task/selectallchildtasks/
---
## Task.SelectAllChildTasks method

Recursively collects all child tasks of this task.

```csharp
public IEnumerable<Task> SelectAllChildTasks()
```

### Return Value

A list of child tasks of this task.

## Examples

Shows how to iterate over child tasks.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task 1");
task.Children.Add("Task 2");

foreach (var tsk in project.RootTask.SelectAllChildTasks())
{
    Console.WriteLine("{0} {1}", tsk.Get(Tsk.Id), tsk.Get(Tsk.Name));
}
```

### See Also

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


