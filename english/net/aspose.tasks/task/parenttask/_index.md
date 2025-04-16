---
title: Task.ParentTask
second_title: Aspose.Tasks for .NET API Reference
description: Task property. Gets the parent task of a task
type: docs
weight: 940
url: /net/aspose.tasks/task/parenttask/
---
## Task.ParentTask property

Gets the parent task of a task.

```csharp
public Task ParentTask { get; }
```

## Examples

Shows how to use the parent task of a task.

```csharp
var project = new Project();
var parent = project.RootTask.Children.Add("Parent");
var child1 = parent.Children.Add("Child1");
var child2 = child1.ParentTask.Children.Add("Child2");

Console.WriteLine("Is parent is equal to the root task: " + child2.ParentTask.Equals(parent));
```

### See Also

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


