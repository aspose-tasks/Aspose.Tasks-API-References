---
title: "Tsk.OvertimeCost"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Il costo totale degli straordinari per un'attività per una risorsa su tutte le attività assegnate o per un'assegnazione di risorsa"
type: docs
weight: 860
url: /it/net/aspose.tasks/tsk/overtimecost/
---
## Tsk.OvertimeCost field

Il costo totale degli straordinari per un'attività, per una risorsa su tutte le attività assegnate o per un'assegnazione di risorsa.

```csharp
public static readonly Key<decimal, TaskKey> OvertimeCost;
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
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


