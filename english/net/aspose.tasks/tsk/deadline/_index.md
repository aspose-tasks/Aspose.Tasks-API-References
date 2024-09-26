---
title: Tsk.Deadline
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. A target date that indicates when a task is to be completed
type: docs
weight: 270
url: /net/aspose.tasks/tsk/deadline/
---
## Tsk.Deadline field

A target date that indicates when a task is to be completed.

```csharp
public static readonly Key<DateTime, TaskKey> Deadline;
```

## Examples

Shows how to read/write Tsk.Deadline property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Deadline, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Deadline: " + task.Get(Tsk.Deadline));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


