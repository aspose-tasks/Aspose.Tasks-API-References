---
title: Task.OutlineOutdent
second_title: Aspose.Tasks for .NET API Reference
description: Task method. Promotes a task in the outline
type: docs
weight: 1390
url: /net/aspose.tasks/task/outlineoutdent/
---
## Task.OutlineOutdent method

Promotes a task in the outline.

```csharp
public void OutlineOutdent()
```

## Examples

Shows how to outdent a task.

```csharp
var project = new Project();
var task1 = project.RootTask.Children.Add("Parent");
var task2 = task1.Children.Add("Task");
Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));

// outdent the task
task2.OutlineOutdent();

Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));
```

### See Also

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


