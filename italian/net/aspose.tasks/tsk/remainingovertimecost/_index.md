---
title: "Tsk.RemainingOvertimeCost"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. La spesa di straordinario programmata rimanente per un'attività."
type: docs
weight: 970
url: /it/net/aspose.tasks/tsk/remainingovertimecost/
---
## Tsk.RemainingOvertimeCost field

La spesa di straordinario programmata rimanente per un'attività.

```csharp
public static readonly Key<decimal, TaskKey> RemainingOvertimeCost;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.RemainingOvertimeCost.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingOvertimeCost, 2m);

Console.WriteLine("Remaining Overtime Cost: " + task.Get(Tsk.RemainingOvertimeCost));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


