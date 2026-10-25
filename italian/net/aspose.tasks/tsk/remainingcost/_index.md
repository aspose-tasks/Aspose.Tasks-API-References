---
title: "Tsk.RemainingCost"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. La spesa programmata rimanente che sarà sostenuta nel completare il lavoro programmato rimanente"
type: docs
weight: 950
url: /it/net/aspose.tasks/tsk/remainingcost/
---
## Tsk.RemainingCost field

La spesa programmata rimanente che sarà sostenuta nel completare il lavoro programmato rimanente.

```csharp
public static readonly Key<decimal, TaskKey> RemainingCost;
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


