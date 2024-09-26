---
title: Tsk.ActualOvertimeWork
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The actual amount of overtime work already performed by resources assigned to tasks
type: docs
weight: 60
url: /net/aspose.tasks/tsk/actualovertimework/
---
## Tsk.ActualOvertimeWork field

The actual amount of overtime work already performed by resources assigned to tasks.

```csharp
public static readonly Key<Duration, TaskKey> ActualOvertimeWork;
```

## Examples

Shows how to read/write Tsk.ActualOvertimeWork property.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualOvertimeWork, project.GetWork(1));

Console.WriteLine("Actual Overtime Work: " + task.Get(Tsk.ActualOvertimeWork));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


