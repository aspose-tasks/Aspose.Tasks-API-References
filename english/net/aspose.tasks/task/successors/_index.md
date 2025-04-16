---
title: Task.Successors
second_title: Aspose.Tasks for .NET API Reference
description: Task property. Gets a TaskCollection object which contains all successors of this Task object
type: docs
weight: 1200
url: /net/aspose.tasks/task/successors/
---
## Task.Successors property

Gets a [`TaskCollection`](../../taskcollection/) object which contains all successors of this Task object.

```csharp
public TaskCollection Successors { get; }
```

### Return Value

Read-only instance of [`TaskCollection`](../../taskcollection/) class.

## Examples

Shows how to read task's successors.

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

### See Also

* class [TaskCollection](../../taskcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


