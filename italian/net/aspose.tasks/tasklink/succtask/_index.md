---
title: "TaskLink.SuccTask"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "TaskLink proprietà. Ottiene o imposta l'attività successiva"
type: docs
weight: 80
url: /it/net/aspose.tasks/tasklink/succtask/
---
## TaskLink.SuccTask property

Ottiene o imposta l'attività successiva.

```csharp
public Task SuccTask { get; set; }
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


