---
title: Tsk.IgnoreWarnings
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. Indicates whether to hide the schedule conflict warning indicator in Microsoft Project
type: docs
weight: 540
url: /net/aspose.tasks/tsk/ignorewarnings/
---
## Tsk.IgnoreWarnings field

Indicates whether to hide the schedule conflict warning indicator in Microsoft Project.

```csharp
public static readonly Key<bool, TaskKey> IgnoreWarnings;
```

## Examples

Shows how to read/write Tsk.IgnoreWarnings property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IgnoreWarnings, true);

Console.WriteLine("Ignore Warnings: " + task.Get(Tsk.IgnoreWarnings));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


