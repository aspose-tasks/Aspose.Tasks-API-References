---
title: Tsk.DisplayAsSummary
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. Determines whether the task should be displayed as a summary task. Reading supported for XML format only
type: docs
weight: 280
url: /net/aspose.tasks/tsk/displayassummary/
---
## Tsk.DisplayAsSummary field

Determines whether the task should be displayed as a summary task. Reading supported for XML format only.

```csharp
public static readonly Key<NullableBool, TaskKey> DisplayAsSummary;
```

## Examples

Shows how to read/write Tsk.DisplayAsSummary property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DisplayAsSummary, true);

Console.WriteLine("Display As Summary: " + task.Get(Tsk.DisplayAsSummary));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


