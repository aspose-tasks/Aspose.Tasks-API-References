---
title: "Tsk.FixedCost"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Mostra qualsiasi spesa di attività non legata a risorse"
type: docs
weight: 430
url: /it/net/aspose.tasks/tsk/fixedcost/
---
## Tsk.FixedCost field

Mostra eventuali spese di attività non legate a risorse.

```csharp
public static readonly Key<double, TaskKey> FixedCost;
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


