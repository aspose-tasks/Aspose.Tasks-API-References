---
title: Task.ParentProject
second_title: Aspose.Tasks for .NET API Reference
description: Task property. Gets the parent project of a task
type: docs
weight: 930
url: /net/aspose.tasks/task/parentproject/
---
## Task.ParentProject property

Gets the parent project of a task.

```csharp
public Project ParentProject { get; }
```

## Remarks

Call Project.UpdateReferences to update these properties.

## Examples

Shows how to use parent project of task.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Parent");

// set a duration for the task by using default project time unit type.
task.Set(Tsk.Duration, task.ParentProject.GetDuration(1));

Console.WriteLine(task.Get(Tsk.Duration));
```

### See Also

* class [Project](../../project/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


