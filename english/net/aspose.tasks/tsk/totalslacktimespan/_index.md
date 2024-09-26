---
title: Tsk.TotalSlackTimeSpan
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The time a tasks finish date can be delayed without delaying the projects finish date
type: docs
weight: 1090
url: /net/aspose.tasks/tsk/totalslacktimespan/
---
## Tsk.TotalSlackTimeSpan field

The time a task's finish date can be delayed without delaying the project's finish date.

```csharp
public static readonly Key<TimeSpan, TaskKey> TotalSlackTimeSpan;
```

## Examples

Shows how to read Tsk.TotalSlackTimeSpan property. The property is calculated, so usually there is no need to set it explicitly.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Total Slack: " + task.Get(Tsk.TotalSlackTimeSpan));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


