---
title: "Tsk.ACWP"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Costi sostenuti per il lavoro già svolto su un'attività fino alla data di stato del progetto o alla data odierna"
type: docs
weight: 110
url: /it/net/aspose.tasks/tsk/acwp/
---
## Tsk.ACWP field

Costi sostenuti per il lavoro già svolto su un'attività, fino alla data di stato del progetto o alla data odierna.

```csharp
public static readonly Key<double, TaskKey> ACWP;
```

## Esempi

Mostra come leggere i valori dei costi delle attività.

```csharp
var project = new Project(DataDir + "ResourceAssignmentCosts.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

foreach (var task in collector.Tasks)
{
    Console.WriteLine("Cost: " + task.Get(Tsk.Cost));
    Console.WriteLine("ACWP: " + task.Get(Tsk.ACWP));
    Console.WriteLine("BCWP: " + task.Get(Tsk.BCWP));
    Console.WriteLine("BCWS: " + task.Get(Tsk.BCWS));

    // CV = BCWP - ACWP
    Console.WriteLine("CV: " + task.Get(Tsk.CV));
    Console.WriteLine();
}
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


