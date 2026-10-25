---
title: "TaskLink.PredTask"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "TaskLink proprietà. Ottiene o imposta l'attività predecessore"
type: docs
weight: 70
url: /it/net/aspose.tasks/tasklink/predtask/
---
## TaskLink.PredTask property

Ottiene o imposta l'attività predecessore.

```csharp
public Task PredTask { get; set; }
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

* class [Task](../../task/)
* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


