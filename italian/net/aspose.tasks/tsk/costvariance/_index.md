---
title: "Tsk.CostVariance"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. La differenza tra il costo di base e il costo totale per una risorsa o un'assegnazione di attività."
type: docs
weight: 240
url: /it/net/aspose.tasks/tsk/costvariance/
---
## Tsk.CostVariance field

La differenza tra il costo di base e il costo totale per un'attività, una risorsa o un'assegnazione.

```csharp
public static readonly Key<double, TaskKey> CostVariance;
```

## Esempi

Mostra come leggere i costi del compito.

```csharp
var project = new Project();

// Aggiungi un compito e imposta il costo
var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Cost, 800);

// Visualizza le proprietà correlate ai costi del compito
Console.WriteLine(task.Get(Tsk.RemainingCost));
Console.WriteLine(task.Get(Tsk.FixedCost));
Console.WriteLine(task.Get(Tsk.CostVariance));
Console.WriteLine(project.RootTask.Get(Tsk.Cost));
Console.WriteLine(project.RootTask.Get(Tsk.FixedCost));
Console.WriteLine(project.RootTask.Get(Tsk.RemainingCost));
Console.WriteLine(project.RootTask.Get(Tsk.CostVariance));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


