---
title: "SplitPart.GetHashCode"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo SplitPart. Restituisce un valore di hash code per l'istanza della classe SplitPart"
type: docs
weight: 40
url: /it/net/aspose.tasks/splitpart/gethashcode/
---
## SplitPart.GetHashCode method

Restituisce un valore di hash code per l'istanza della classe [`SplitPart`](../).

```csharp
public override int GetHashCode()
```

### Valore di ritorno

restituisce un valore di hash per questo oggetto.

## Esempi

Mostra come ottenere un hash code di una parte divisa.

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

// L'uguaglianza delle parti divise viene verificata rispetto a inizio, fine e indice delle parti divise.
var part1 = task.SplitParts[0];
var part2 = task.SplitParts[1];

// Il valore di hash code di una parte divisa basato su inizio, fine e indice di una parte divisa.
Console.WriteLine("Split Part 1 Start {0} Finish {1} HashCode {2}", part1.Start, part1.Finish, part1.GetHashCode());
Console.WriteLine("Split Part 2 Start {0} Finish {1} HashCode {2}", part2.Start, part2.Finish, part2.GetHashCode());
```

### Vedi anche

* class [SplitPart](../)
* namespace [Aspose.Tasks](../../splitpart/)
* assembly [Aspose.Tasks](../../../)


