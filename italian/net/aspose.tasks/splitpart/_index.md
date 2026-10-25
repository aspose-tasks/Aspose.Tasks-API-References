---
title: "Classe SplitPart"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.SplitPart. Rappresenta una porzione di attività. SplitPart è un membro della collezione SplitParts delle attività."
type: docs
weight: 2290
url: /it/net/aspose.tasks/splitpart/
---
## SplitPart class

Rappresenta una porzione di attività. Lo SplitPart è un membro della collezione SplitParts dell'attività.

```csharp
public class SplitPart
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Finish](../../aspose.tasks/splitpart/finish/) { get; } | Ottiene la data di fine di uno SplitPart. |
| [Start](../../aspose.tasks/splitpart/start/) { get; } | Ottiene la data di inizio di uno SplitPart. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [Equals](../../aspose.tasks/splitpart/equals/)(object) | Confronta due parti divise. |
| override [GetHashCode](../../aspose.tasks/splitpart/gethashcode/)() | Restituisce un valore di hash code per l'istanza della classe `SplitPart`. |

## Esempi

Mostra come lavorare con le parti divise di un'attività suddivisa.

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

// devi prima generare i dati a tempo dell'assegnazione delle risorse
assignment.TimephasedDataFromTaskDuration(project.Get(Prj.Calendar));

// dividi l'attività.
assignment.SplitTask(new DateTime(2000, 3, 16, 8, 0, 0), new DateTime(2000, 3, 17, 17, 0, 0), project.Get(Prj.Calendar));

// itera sulle parti divise
Console.WriteLine("Number of split parts: " + task.SplitParts.Count);
foreach (var splitPart in task.SplitParts)
{
    Console.WriteLine("  Split Part Start: " + splitPart.Start);
    Console.WriteLine("  Split Part Finish: " + splitPart.Finish);
    Console.WriteLine();
}
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


