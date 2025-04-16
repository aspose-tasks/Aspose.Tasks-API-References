---
title: Task.OutlineIndent
second_title: Aspose.Tasks for .NET API Reference
description: Task method. Indents a task in the outline
type: docs
weight: 1380
url: /net/aspose.tasks/task/outlineindent/
---
## Task.OutlineIndent method

Indents a task in the outline.

```csharp
public void OutlineIndent()
```

## Examples

Shows how to indent a task.

```csharp
var project = new Project();
var task1 = project.RootTask.Children.Add("Parent");
var task2 = project.RootTask.Children.Add("Task");
Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));

// indent the task
task2.OutlineIndent();

Console.WriteLine("Outline Level: " + task1.Get(Tsk.OutlineLevel));
Console.WriteLine("Outline Level: " + task2.Get(Tsk.OutlineLevel));
```

### See Also

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


