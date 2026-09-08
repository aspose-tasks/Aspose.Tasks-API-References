---
title: "SplitPart.Finish"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "SplitPart eigenschap. Haalt de einddatum van een SplitPart op"
type: docs
weight: 10
url: /nl/net/aspose.tasks/splitpart/finish/
---
## SplitPart.Finish property

Haalt de einddatum op van een SplitPart.

```csharp
public DateTime Finish { get; }
```

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

* class [SplitPart](../)
* namespace [Aspose.Tasks](../../splitpart/)
* assembly [Aspose.Tasks](../../../)


