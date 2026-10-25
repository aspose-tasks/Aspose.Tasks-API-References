---
title: "Tsk.OvertimeWork"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. La quantità di straordinario programmata da eseguire da tutte le risorse assegnate a un'attività"
type: docs
weight: 870
url: /it/net/aspose.tasks/tsk/overtimework/
---
## Tsk.OvertimeWork field

La quantità di straordinario programmata da eseguire da tutte le risorse assegnate a un'attività.

```csharp
public static readonly Key<Duration, TaskKey> OvertimeWork;
```

## Esempi

Mostra come leggere gli straordinari delle attività.

```csharp
var project = new Project(DataDir + "TaskOvertimes.mpp");

// Leggi gli straordinari e la percentuale di completamento per le attività
foreach (var task in project.RootTask.Children)
{
    Console.WriteLine(task.Get(Tsk.OvertimeCost));
    Console.WriteLine(task.Get(Tsk.OvertimeWork));
    Console.WriteLine(task.Get(Tsk.PercentComplete));
    Console.WriteLine(task.Get(Tsk.PercentWorkComplete));
    Console.WriteLine(task.Get(Tsk.PhysicalPercentComplete));

    // Imposta la percentuale completata
    task.Set(Tsk.PercentComplete, 100);
}
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


