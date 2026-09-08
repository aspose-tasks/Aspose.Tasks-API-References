---
title: "Tsk.ActualDuration"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Tsk-veld. Het bereik van de feitelijke werktijd voor een taak, gebaseerd op de geplande duur en het huidige resterende werk of percentage voltooid."
type: docs
weight: 30
url: /nl/net/aspose.tasks/tsk/actualduration/
---
## Tsk.ActualDuration field

De periode van feitelijke werktijd voor een taak, gebaseerd op de geplande duur en het huidige resterende werk of het voltooiingspercentage.

```csharp
public static readonly Key<Duration, TaskKey> ActualDuration;
```

## Voorbeelden

Toont hoe de werkelijke eigenschappen van een taak gelezen kunnen worden.

```csharp
var project = new Project(DataDir + "ActualTaskProperties.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Alle verzamelde taken doorlopen
foreach (var task in collector.Tasks)
{
    Console.WriteLine("Task Name : " + task.Get(Tsk.Name));
    Console.WriteLine("Actual Start: " + task.Get(Tsk.ActualStart).ToLongDateString());
    Console.WriteLine("Actual Finish: " + task.Get(Tsk.ActualFinish).ToLongDateString());
    Console.WriteLine("Actual Duration: " + task.Get(Tsk.ActualDuration).TimeSpan.Hours);
    Console.WriteLine("Actual Cost: " + task.Get(Tsk.ActualCost));
}
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


