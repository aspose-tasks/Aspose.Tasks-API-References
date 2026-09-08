---
title: "TaskLink.LinkLag"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TaskLink eigenschap. Haalt de vertraging op in tienden van een minuut of percentage, of stelt deze in"
type: docs
weight: 40
url: /nl/net/aspose.tasks/tasklink/linklag/
---
## TaskLink.LinkLag property

Haalt een waarde op of stelt deze in voor de vertraging in tienden van een minuut of als percentage.

```csharp
public int LinkLag { get; set; }
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

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


