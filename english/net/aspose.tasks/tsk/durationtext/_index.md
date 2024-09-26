---
title: Tsk.DurationText
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. Returns the tasks duration text
type: docs
weight: 310
url: /net/aspose.tasks/tsk/durationtext/
---
## Tsk.DurationText field

Returns the task's duration text.

```csharp
public static readonly Key<string, TaskKey> DurationText;
```

## Examples

Shows how to read/write Tsk.DurationText property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DurationText, "Not A Duration");

Console.WriteLine("Duration Text: " + task.Get(Tsk.DurationText));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


