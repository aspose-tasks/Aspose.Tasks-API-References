---
title: Tsk.FreeSlackTimeSpan
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The time that a task can be delayed without delaying any successor tasks
type: docs
weight: 450
url: /net/aspose.tasks/tsk/freeslacktimespan/
---
## Tsk.FreeSlackTimeSpan field

The time that a task can be delayed without delaying any successor tasks.

```csharp
public static readonly Key<TimeSpan, TaskKey> FreeSlackTimeSpan;
```

## Examples

Shows how to read Tsk.FreeSlackTimeSpan property. The property is calculated, so usually there is no need to set it explicitly.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Free Slack: " + task.Get(Tsk.FreeSlackTimeSpan));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


