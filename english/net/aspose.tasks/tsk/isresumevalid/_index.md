---
title: Tsk.IsResumeValid
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. Determines whether a task can be resumed
type: docs
weight: 680
url: /net/aspose.tasks/tsk/isresumevalid/
---
## Tsk.IsResumeValid field

Determines whether a task can be resumed.

```csharp
public static readonly Key<NullableBool, TaskKey> IsResumeValid;
```

## Examples

Shows how to read/write Tsk.IsResumeValid property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsResumeValid, true);

Console.WriteLine("Is Resume Valid: " + task.Get(Tsk.IsResumeValid));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


