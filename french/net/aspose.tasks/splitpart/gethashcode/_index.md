---
title: "SplitPart.GetHashCode"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode SplitPart. Retourne une valeur de code de hachage pour l'instance de la classe SplitPart"
type: docs
weight: 40
url: /fr/net/aspose.tasks/splitpart/gethashcode/
---
## SplitPart.GetHashCode method

Retourne une valeur de code de hachage pour l'instance de la classe [`SplitPart`](../).

```csharp
public override int GetHashCode()
```

### Valeur de retour

retourne une valeur de code de hachage pour cet objet.

## Exemples

Montre comment obtenir le code de hachage d'une partie découpée.

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

// doit d'abord générer les données temporelles d'affectation de ressources
assignment.TimephasedDataFromTaskDuration(project.Get(Prj.Calendar));

// diviser la tâche.
assignment.SplitTask(new DateTime(2000, 3, 16, 8, 0, 0), new DateTime(2000, 3, 17, 17, 0, 0), project.Get(Prj.Calendar));

// L'égalité des parties découpées est vérifiée par rapport au début, à la fin et à l'index des parties découpées.
var part1 = task.SplitParts[0];
var part2 = task.SplitParts[1];

// Le code de hachage d'une partie découpée basé sur le début, la fin et l'index d'une partie découpée.
Console.WriteLine("Split Part 1 Start {0} Finish {1} HashCode {2}", part1.Start, part1.Finish, part1.GetHashCode());
Console.WriteLine("Split Part 2 Start {0} Finish {1} HashCode {2}", part2.Start, part2.Finish, part2.GetHashCode());
```

### Voir aussi

* class [SplitPart](../)
* namespace [Aspose.Tasks](../../splitpart/)
* assembly [Aspose.Tasks](../../../)


