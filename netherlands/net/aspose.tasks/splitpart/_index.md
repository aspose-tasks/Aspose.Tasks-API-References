---
title: "Klasse SplitPart"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.SplitPart klasse. Vertegenwoordigt een taakdeel. De SplitPart is een lid van de SplitParts‑collectie van taken."
type: docs
weight: 2290
url: /nl/net/aspose.tasks/splitpart/
---
## SplitPart class

Stelt een taakdeel voor. De SplitPart is een lid van de SplitParts‑collectie van de taak.

```csharp
public class SplitPart
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Finish](../../aspose.tasks/splitpart/finish/) { get; } | Haalt de einddatum op van een SplitPart. |
| [Start](../../aspose.tasks/splitpart/start/) { get; } | Haalt de startdatum op van een SplitPart. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| override [Equals](../../aspose.tasks/splitpart/equals/)(object) | Vergelijkt twee split‑delen. |
| override [GetHashCode](../../aspose.tasks/splitpart/gethashcode/)() | Retourneert een hash‑codewaarde voor de instantie van de `SplitPart` klasse. |

## Voorbeelden

Toont hoe te werken met split‑delen van een gesplitste taak.

```csharp
var project = new Project();
project.Set(Prj.StartDate, new DateTime(2000, 3, 15, 8, 0, 0));
project.Set(Prj.FinishDate, new DateTime(2000, 3, 21, 17, 0, 0));

var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.IsManual, false);
task.Set(Tsk.Start, new DateTime(2000, 3, 15, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(3));

var assignment = project.ResourceAssignments.Add(task, project.Resources.Add("r1"));
assignment.Set(Asn.Start, new DateTime(2000, 3, 15, 8, 0, 0));
assignment.Set(Asn.Work, task.Get(Tsk.Work));
assignment.Set(Asn.Finish, new DateTime(2000, 3, 19, 17, 0, 0));

// moet eerst resource‑toewijzings‑timephased‑gegevens genereren
assignment.TimephasedDataFromTaskDuration(project.Get(Prj.Calendar));

// splits de taak.
assignment.SplitTask(new DateTime(2000, 3, 16, 8, 0, 0), new DateTime(2000, 3, 17, 17, 0, 0), project.Get(Prj.Calendar));

// itereren over gesplitste delen
Console.WriteLine("Number of split parts: " + task.SplitParts.Count);
foreach (var splitPart in task.SplitParts)
{
    Console.WriteLine("  Split Part Start: " + splitPart.Start);
    Console.WriteLine("  Split Part Finish: " + splitPart.Finish);
    Console.WriteLine();
}
```

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


