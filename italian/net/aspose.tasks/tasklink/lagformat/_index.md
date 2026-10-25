---
title: "TaskLink.LagFormat"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "TaskLink proprietà. Ottiene o imposta il formato per esprimere il formato del ritardo"
type: docs
weight: 30
url: /it/net/aspose.tasks/tasklink/lagformat/
---
## TaskLink.LagFormat property

Ottiene o imposta il formato per esprimere il ritardo.

```csharp
public TimeUnitType LagFormat { get; set; }
```

## Esempi

Mostra come leggere i collegamenti delle attività del progetto.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

// Visualizza i nomi delle attività predecessore e successiva
foreach (var taskLink in project.TaskLinks)
{
    Console.WriteLine("Predecessor: " + taskLink.PredTask.Get(Tsk.Name));
    Console.WriteLine("Successor: " + taskLink.SuccTask.Get(Tsk.Name));
    Console.WriteLine("Lag Format: " + taskLink.LagFormat);
    Console.WriteLine("Link Lag: " + taskLink.LinkLag);
    Console.WriteLine();
}
```

### Vedi anche

* enum [TimeUnitType](../../timeunittype/)
* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


