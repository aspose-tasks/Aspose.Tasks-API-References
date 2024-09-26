---
title: Tsk.Duration
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The total span of active working time for a task as entered or as calculated by Microsoft Project based on start date finish date calendars and other scheduling factors
type: docs
weight: 300
url: /net/aspose.tasks/tsk/duration/
---
## Tsk.Duration field

The total span of active working time for a task as entered or as calculated by Microsoft Project based on start date, finish date, calendars, and other scheduling factors.

```csharp
public static readonly Key<Duration, TaskKey> Duration;
```

## Examples

Shows how to set duration of the task.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.Start, new DateTime(2012, 8, 23, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(24, TimeUnitType.Hour));
task.Set(Tsk.ActualStart, new DateTime(2012, 8, 23, 8, 0, 0));

project.Save(OutDir + "AddTaskDuration_out.xml", SaveFileFormat.Xml);
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


