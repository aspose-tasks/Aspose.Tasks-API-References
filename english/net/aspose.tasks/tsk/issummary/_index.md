---
title: Tsk.IsSummary
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. Determines whether a task is a summary task
type: docs
weight: 720
url: /net/aspose.tasks/tsk/issummary/
---
## Tsk.IsSummary field

Determines whether a task is a summary task.

```csharp
public static readonly Key<bool, TaskKey> IsSummary;
```

## Examples

Shows how to read/write Tsk.IsSummary property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsSummary, true);

Console.WriteLine("Is Summary: " + task.Get(Tsk.IsSummary));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


