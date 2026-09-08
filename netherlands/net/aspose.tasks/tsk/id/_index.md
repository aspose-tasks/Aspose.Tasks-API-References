---
title: "Tsk.Id"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk veld. De positie‑identificatie van een taak binnen de lijst met taken"
type: docs
weight: 520
url: /nl/net/aspose.tasks/tsk/id/
---
## Tsk.Id field

De positie‑identificatie van een taak binnen de takenlijst.

```csharp
public static readonly Key<int, TaskKey> Id;
```

## Voorbeelden

Toont hoe taak‑eigenschappen te lezen/schrijven.

```csharp
var project = new Project();

// Taak toevoegen en taak‑eigenschappen instellen
var task = project.RootTask.Children.Add();
task.Set(Tsk.Name, "Task1");
task.Set(Tsk.Start, new DateTime(2020, 3, 31, 8, 0, 0));
task.Set(Tsk.Finish, new DateTime(2020, 3, 31, 17, 0, 0));

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Alle verzamelde taken doorlopen
foreach (var tsk in collector.Tasks)
{
    Console.WriteLine("Task Id: {0}", tsk.Get(Tsk.Id));
    Console.WriteLine("Task Uid: {0}", tsk.Get(Tsk.Uid));
    Console.WriteLine("Task Name: {0}", tsk.Get(Tsk.Name));
    Console.WriteLine("Task Start: {0}", tsk.Get(Tsk.Start));
    Console.WriteLine("Task Finish: {0}", tsk.Get(Tsk.Finish));
}
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


