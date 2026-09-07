---
title: "Tsk.CV"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. La differenza tra il costo di base e il costo totale per un'attività. Varianza di costo  Costo  Costo di base"
type: docs
weight: 260
url: /it/net/aspose.tasks/tsk/cv/
---
## Tsk.CV field

La differenza tra il costo di base e il costo totale per un'attività. Scostamento di costo = Costo - Costo di base

```csharp
public static readonly Key<double, TaskKey> CV;
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


