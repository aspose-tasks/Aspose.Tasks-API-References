---
title: Tsk.DisplayOnTimeline
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. Specifies whether a task should be displayed on a timeline view
type: docs
weight: 290
url: /net/aspose.tasks/tsk/displayontimeline/
---
## Tsk.DisplayOnTimeline field

Specifies whether a task should be displayed on a timeline view.

```csharp
public static readonly Key<bool, TaskKey> DisplayOnTimeline;
```

## Examples

Shows how to read/write Tsk.DisplayOnTimeline property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.DisplayOnTimeline, true);

Console.WriteLine("Display On Timeline: " + task.Get(Tsk.DisplayOnTimeline));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


