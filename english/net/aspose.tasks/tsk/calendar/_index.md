---
title: Tsk.Calendar
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. The task calendar
type: docs
weight: 160
url: /net/aspose.tasks/tsk/calendar/
---
## Tsk.Calendar field

The task calendar.

```csharp
public static readonly Key<Calendar, TaskKey> Calendar;
```

## Examples

Shows how to read/write task calendars.

```csharp
var project = new Project(DataDir + "ReadTaskCalendar.mpp");
var task = project.RootTask.Children.Add("Task1");

// Create calendar and assign to task
var newCalendar = project.Calendars.Add("TaskCal1");
task.Set(Tsk.Calendar, newCalendar);

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Parse all the recursive children
foreach (var tsk in collector.Tasks)
{
    var calendar = tsk.Get(Tsk.Calendar);
    Console.WriteLine("Task calendar name: {0}", calendar == null ? "None" : calendar.Name);
}
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Calendar](../../calendar/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


