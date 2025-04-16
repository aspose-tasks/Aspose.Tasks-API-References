---
title: Task.Delete
second_title: Aspose.Tasks for .NET API Reference
description: Task method. Deletes a task from parent project tasks collection and all its assignments
type: docs
weight: 1320
url: /net/aspose.tasks/task/delete/
---
## Task.Delete method

Deletes a task from parent project tasks collection and all its assignments.

```csharp
public void Delete()
```

## Examples

Shows how to delete a task.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Number of tasks: " + project.RootTask.Children.Count);

// delete a task
task.Delete();

Console.WriteLine("Number of tasks: " + project.RootTask.Children.Count);
```

### See Also

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


