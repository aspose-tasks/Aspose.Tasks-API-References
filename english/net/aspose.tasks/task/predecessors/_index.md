---
title: Task.Predecessors
second_title: Aspose.Tasks for .NET API Reference
description: Task property. Gets a TaskCollection object which contains all predecessors of this Task object
type: docs
weight: 980
url: /net/aspose.tasks/task/predecessors/
---
## Task.Predecessors property

Gets a [`TaskCollection`](../../taskcollection/) object which contains all predecessors of this Task object.

```csharp
public TaskCollection Predecessors { get; }
```

### Return Value

Read-only instance of [`TaskCollection`](../../taskcollection/) class.

## Examples

Shows how to read task's predecessors.

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

### See Also

* class [TaskCollection](../../taskcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


