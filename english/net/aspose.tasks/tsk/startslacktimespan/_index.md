---
title: Tsk.StartSlackTimeSpan
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The duration between the Early Start and Late Start dates
type: docs
weight: 1020
url: /net/aspose.tasks/tsk/startslacktimespan/
---
## Tsk.StartSlackTimeSpan field

The duration between the Early Start and Late Start dates.

```csharp
public static readonly Key<TimeSpan, TaskKey> StartSlackTimeSpan;
```

## Examples

Shows how to read Tsk.StartSlackTimeSpan property. The property is calculated, so usually there is no need to set it explicitly.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

Console.WriteLine("Start Slack: " + task.Get(Tsk.StartSlackTimeSpan));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


