---
title: Tsk.IgnoreResourceCalendar
second_title: Aspose.Tasks for .NET API Reference
description: Tsk field. Determines whether the scheduling of the task considers the calendars of the resources assigned to the task
type: docs
weight: 530
url: /net/aspose.tasks/tsk/ignoreresourcecalendar/
---
## Tsk.IgnoreResourceCalendar field

Determines whether the scheduling of the task considers the calendars of the resources assigned to the task.

```csharp
public static readonly Key<NullableBool, TaskKey> IgnoreResourceCalendar;
```

## Examples

Shows how to read/write Tsk.IgnoreResourceCalendar property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IgnoreResourceCalendar, true);

Console.WriteLine("Ignore Resource Calendar: " + task.Get(Tsk.IgnoreResourceCalendar));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


