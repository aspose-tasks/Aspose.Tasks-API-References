---
title: "Task.Status"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Task. Ottiene lo stato dell'attività"
type: docs
weight: 1160
url: /it/net/aspose.tasks/task/status/
---
## Task.Status property

Ottiene lo stato dell'attività.

```csharp
public TaskStatus Status { get; }
```

## Esempi

Mostra come ottenere lo stato dell'attività.

```csharp
var project = new Project(DataDir + "TaskPercentageCompletion.mpp");

// La data di stato del progetto dovrebbe essere impostata perché il calcolo dello stato utilizza la data di stato.
project.StatusDate = new DateTime(2010, 7, 9, 15, 0, 0);
foreach (var task in project.EnumerateAllChildTasks())
{
    Console.WriteLine("{0} - {1}", task.Name, task.Status);
}
```

### Vedi anche

* enum [TaskStatus](../../taskstatus/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


