---
title: "SplitPart.GetHashCode"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "SplitPart-methode. Retourneert een hashcode‑waarde voor de instantie van de SplitPart‑klasse."
type: docs
weight: 40
url: /nl/net/aspose.tasks/splitpart/gethashcode/
---
## SplitPart.GetHashCode method

Retourneert een hashcode‑waarde voor de instantie van de [`SplitPart`](../)‑klasse.

```csharp
public override int GetHashCode()
```

### Retourwaarde

retourneert een hashcodewaarde voor dit object.

## Voorbeelden

Toont hoe een hashcode van een split part te verkrijgen.

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

// De gelijkheid van split parts wordt gecontroleerd ten opzichte van start, einde en index van split parts.
var part1 = task.SplitParts[0];
var part2 = task.SplitParts[1];

// De hashcode van een split part gebaseerd op start, einde en index van een split part.
Console.WriteLine("Split Part 1 Start {0} Finish {1} HashCode {2}", part1.Start, part1.Finish, part1.GetHashCode());
Console.WriteLine("Split Part 2 Start {0} Finish {1} HashCode {2}", part2.Start, part2.Finish, part2.GetHashCode());
```

### Zie ook

* class [SplitPart](../)
* namespace [Aspose.Tasks](../../splitpart/)
* assembly [Aspose.Tasks](../../../)


