---
title: "TaskLink.LagFormat"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TaskLink eigenschap. Haalt het formaat voor het uitdrukken van de vertraging op of stelt dit in"
type: docs
weight: 30
url: /nl/net/aspose.tasks/tasklink/lagformat/
---
## TaskLink.LagFormat property

Haalt een waarde op of stelt deze in voor het formaat waarmee de vertraging wordt weergegeven.

```csharp
public TimeUnitType LagFormat { get; set; }
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

* enum [TimeUnitType](../../timeunittype/)
* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


