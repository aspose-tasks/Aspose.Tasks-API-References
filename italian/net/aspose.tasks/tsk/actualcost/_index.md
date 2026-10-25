---
title: "Tsk.ActualCost"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Costi sostenuti per il lavoro già svolto dalle risorse sulle loro attività insieme a qualsiasi altro costo registrato associato all'attività"
type: docs
weight: 20
url: /it/net/aspose.tasks/tsk/actualcost/
---
## Tsk.ActualCost field

Costi sostenuti per il lavoro già eseguito dalle risorse sui loro compiti, insieme a qualsiasi altro costo registrato associato al compito.

```csharp
public static readonly Key<decimal, TaskKey> ActualCost;
```

## Esempi

Mostra come leggere le proprietà effettive dell'attività.

```csharp
var project = new Project(DataDir + "ActualTaskProperties.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// Analizza tutti i task raccolti
foreach (var task in collector.Tasks)
{
    Console.WriteLine("Task Name : " + task.Get(Tsk.Name));
    Console.WriteLine("Actual Start: " + task.Get(Tsk.ActualStart).ToLongDateString());
    Console.WriteLine("Actual Finish: " + task.Get(Tsk.ActualFinish).ToLongDateString());
    Console.WriteLine("Actual Duration: " + task.Get(Tsk.ActualDuration).TimeSpan.Hours);
    Console.WriteLine("Actual Cost: " + task.Get(Tsk.ActualCost));
}
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


