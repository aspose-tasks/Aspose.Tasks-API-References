---
title: "TaskLink.SuccTask"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TaskLink eigenschap. Haalt de opvolger taak op of stelt deze in"
type: docs
weight: 80
url: /nl/net/aspose.tasks/tasklink/succtask/
---
## TaskLink.SuccTask property

Haalt een waarde op of stelt deze in voor de opvolger‑taak.

```csharp
public Task SuccTask { get; set; }
```

## Voorbeelden

Toont hoe projecttaak‑koppelingen te lezen.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

// Geef de namen weer van voorganger‑ en opvolger‑taken
foreach (var taskLink in project.TaskLinks)
{
    Console.WriteLine("Predecessor: " + taskLink.PredTask.Get(Tsk.Name));
    Console.WriteLine("Successor: " + taskLink.SuccTask.Get(Tsk.Name));
    Console.WriteLine("Lag Format: " + taskLink.LagFormat);
    Console.WriteLine("Link Lag: " + taskLink.LinkLag);
    Console.WriteLine();
}
```

### Zie ook

* class [Task](../../task/)
* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


