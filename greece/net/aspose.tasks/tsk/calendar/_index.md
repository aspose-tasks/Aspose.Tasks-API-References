---
title: "Tsk.Calendar"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Tsk. Το ημερολόγιο της εργασίας"
type: docs
weight: 160
url: /el/net/aspose.tasks/tsk/calendar/
---
## Tsk.Calendar field

Το ημερολόγιο του έργου.

```csharp
public static readonly Key<Calendar, TaskKey> Calendar;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε ημερολόγια εργασιών.

```csharp
var project = new Project(DataDir + "ReadTaskCalendar.mpp");
var task = project.RootTask.Children.Add("Task1");

// Δημιουργήστε ημερολόγιο και εκχωρήστε το στην εργασία
var newCalendar = project.Calendars.Add("TaskCal1");
task.Set(Tsk.Calendar, newCalendar);

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Αναλύστε όλα τα αναδρομικά παιδιά
foreach (var tsk in collector.Tasks)
{
    var calendar = tsk.Get(Tsk.Calendar);
    Console.WriteLine("Task calendar name: {0}", calendar == null ? "None" : calendar.Name);
}
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Calendar](../../calendar/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


