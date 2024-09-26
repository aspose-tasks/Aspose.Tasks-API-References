---
title: Tsk.FinishSlackTimeSpan
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The duration between the Early Finish and Late Finish dates
type: docs
weight: 400
url: /net/aspose.tasks/tsk/finishslacktimespan/
---
## Tsk.FinishSlackTimeSpan field

The duration between the Early Finish and Late Finish dates.

```csharp
public static readonly Key<TimeSpan, TaskKey> FinishSlackTimeSpan;
```

## Examples

Shows how to read Tsk.FinishSlackTimeSpan property. The property is calculated, so usually there is no need to set it explicitly.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Finish Slack: " + task.Get(Tsk.FinishSlackTimeSpan));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


