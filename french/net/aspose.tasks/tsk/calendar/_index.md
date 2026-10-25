---
title: "Tsk.Calendar"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Le calendrier de la tâche"
type: docs
weight: 160
url: /fr/net/aspose.tasks/tsk/calendar/
---
## Tsk.Calendar field

Le calendrier de la tâche.

```csharp
public static readonly Key<Calendar, TaskKey> Calendar;
```

## Exemples

Montre comment lire/écrire les calendriers de tâches.

```csharp
var project = new Project(DataDir + "ReadTaskCalendar.mpp");
var task = project.RootTask.Children.Add("Task1");

// Créer un calendrier et l'assigner à la tâche
var newCalendar = project.Calendars.Add("TaskCal1");
task.Set(Tsk.Calendar, newCalendar);

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Analyser tous les enfants récursifs
foreach (var tsk in collector.Tasks)
{
    var calendar = tsk.Get(Tsk.Calendar);
    Console.WriteLine("Task calendar name: {0}", calendar == null ? "None" : calendar.Name);
}
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Calendar](../../calendar/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


