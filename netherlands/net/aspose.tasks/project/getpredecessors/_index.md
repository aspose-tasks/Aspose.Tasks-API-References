---
title: "Project.GetPredecessors"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Project methode. Retourneert een verzameling van taaklinks die voorgangers zijn van de opgegeven taak"
type: docs
weight: 1120
url: /nl/net/aspose.tasks/project/getpredecessors/
---
## Project.GetPredecessors method

Retourneert een verzameling taaklinks die voorlopers zijn van de opgegeven taak.

```csharp
public TaskLinkCollection GetPredecessors(Task task)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| taak | Taak | De taak waarvoor de voorgangers opgehaald moeten worden. |

### Retourwaarde

Lijst van voorgangers [`TaskLink`](../../tasklink/).

## Voorbeelden

Toont hoe voorgangers voor de specifieke taak opgehaald kunnen worden.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");
var task = project.RootTask.Children.GetById(10);

var predecessors = project.GetPredecessors(task);

// Geef de namen weer van voorganger‑ en opvolger‑taken
foreach (var predecessor in predecessors)
{
    Console.WriteLine("Predecessor " + predecessor.PredTask.Get(Tsk.Name));
    Console.WriteLine("Successor " + predecessor.SuccTask.Get(Tsk.Name));
}
```

### Zie ook

* class [TaskLinkCollection](../../tasklinkcollection/)
* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


