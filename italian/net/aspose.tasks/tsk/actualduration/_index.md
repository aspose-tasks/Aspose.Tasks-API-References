---
title: "Tsk.ActualDuration"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. L'intervallo di tempo di lavoro effettivo per un'attività basato sulla durata programmata e sul lavoro rimanente corrente o sulla percentuale completata."
type: docs
weight: 30
url: /it/net/aspose.tasks/tsk/actualduration/
---
## Tsk.ActualDuration field

L'intervallo di tempo di lavoro effettivo per un'attività, basato sulla durata pianificata e sul lavoro rimanente attuale o sulla percentuale di completamento.

```csharp
public static readonly Key<Duration, TaskKey> ActualDuration;
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
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


