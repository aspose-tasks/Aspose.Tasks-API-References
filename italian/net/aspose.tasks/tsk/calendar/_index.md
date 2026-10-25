---
title: "Tsk.Calendar"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Il calendario del compito"
type: docs
weight: 160
url: /it/net/aspose.tasks/tsk/calendar/
---
## Tsk.Calendar field

Il calendario dell'attività.

```csharp
public static readonly Key<Calendar, TaskKey> Calendar;
```

## Esempi

Mostra come leggere/scrivere i calendari dei compiti.

```csharp
var project = new Project(DataDir + "ReadTaskCalendar.mpp");
var task = project.RootTask.Children.Add("Task1");

// Crea un calendario e assegnalo al compito
var newCalendar = project.Calendars.Add("TaskCal1");
task.Set(Tsk.Calendar, newCalendar);

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Analizza tutti i figli ricorsivi
foreach (var tsk in collector.Tasks)
{
    var calendar = tsk.Get(Tsk.Calendar);
    Console.WriteLine("Task calendar name: {0}", calendar == null ? "None" : calendar.Name);
}
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Calendar](../../calendar/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


