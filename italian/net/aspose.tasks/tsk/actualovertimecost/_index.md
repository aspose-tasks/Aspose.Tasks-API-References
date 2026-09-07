---
title: "Tsk.ActualOvertimeCost"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Tsk. Costi sostenuti per lavoro straordinario già eseguito sulle attività dalle risorse assegnate"
type: docs
weight: 50
url: /it/net/aspose.tasks/tsk/actualovertimecost/
---
## Tsk.ActualOvertimeCost field

Costi sostenuti per il lavoro straordinario già svolto sui task dalle risorse assegnate.

```csharp
public static readonly Key<decimal, TaskKey> ActualOvertimeCost;
```

## Esempi

Mostra come leggere/scrivere la proprietà Tsk.ActualOvertimeCost.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualOvertimeCost, 10m);

Console.WriteLine("Actual Overtime Cost: " + task.Get(Tsk.ActualOvertimeCost));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


