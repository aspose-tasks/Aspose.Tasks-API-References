---
title: Tsk.Type
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The type of a task
type: docs
weight: 1100
url: /net/aspose.tasks/tsk/type/
---
## Tsk.Type field

The type of a task.

```csharp
public static readonly Key<TaskType, TaskKey> Type;
```

## Examples

Shows how to read/write Tsk.Type property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Type, TaskType.FixedDuration);

Console.WriteLine("Type: " + task.Get(Tsk.Type));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskType](../../tasktype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


