---
title: "Klasse TaskLink"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.TaskLink‑klasse. Vertegenwoordigt een voorganger‑koppeling"
type: docs
weight: 2410
url: /nl/net/aspose.tasks/tasklink/
---
## TaskLink class

Stelt een voorgangerkoppeling voor.

```csharp
public sealed class TaskLink : IEquatable<TaskLink>
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [CrossProjectName](../../aspose.tasks/tasklink/crossprojectname/) { get; set; } | Haalt een waarde op of stelt deze in voor het externe voorgangerproject. |
| [IsCrossProject](../../aspose.tasks/tasklink/iscrossproject/) { get; set; } | Haalt een waarde op of stelt deze in die aangeeft of een voorganger deel uitmaakt van een ander project. |
| [LagFormat](../../aspose.tasks/tasklink/lagformat/) { get; set; } | Haalt een waarde op of stelt deze in voor het formaat waarmee de vertraging wordt weergegeven. |
| [LinkLag](../../aspose.tasks/tasklink/linklag/) { get; set; } | Haalt een waarde op of stelt deze in voor de vertraging in tienden van een minuut of als percentage. |
| [LinkLagTimeSpan](../../aspose.tasks/tasklink/linklagtimespan/) { get; set; } | Haalt een waarde op of stelt deze in voor de duur van de vertraging, afhankelijk van LagFormat. |
| [LinkType](../../aspose.tasks/tasklink/linktype/) { get; set; } | Haalt een waarde op of stelt deze in voor het type van een koppeling. |
| [PredTask](../../aspose.tasks/tasklink/predtask/) { get; set; } | Haalt een waarde op of stelt deze in voor de voorganger‑taak. |
| [SuccTask](../../aspose.tasks/tasklink/succtask/) { get; set; } | Haalt een waarde op of stelt deze in voor de opvolger‑taak. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| override [Equals](../../aspose.tasks/tasklink/equals/#equals_1)(object) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| [Equals](../../aspose.tasks/tasklink/equals/#equals)(TaskLink) | Retourneert een waarde die aangeeft of deze instantie gelijk is aan een opgegeven object. |
| override [GetHashCode](../../aspose.tasks/tasklink/gethashcode/)() | Retourneert een hashcode‑waarde voor de instantie van de `TaskLink`‑klasse. |
| override [ToString](../../aspose.tasks/tasklink/tostring/)() | Retourneert de tekenreeksrepresentatie van een TaskLink. De exacte details van de representatie zijn niet gespecificeerd en kunnen wijzigen. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


