---
title: "SplitPart.Equals"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode SplitPart. Compare deux parties découpées"
type: docs
weight: 30
url: /fr/net/aspose.tasks/splitpart/equals/
---
## SplitPart.Equals method

Compare deux parties découpées.

```csharp
public override bool Equals(object obj)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| obj | Objet | Objet à comparer. |

### Valeur de retour

Vrai si l'objet spécifié est égal à l'objet actuel ; sinon, faux.

## Exemples

Montre comment vérifier l'égalité des parties découpées.

```csharp
var project = new Project();
project.Set(Prj.StartDate, new DateTime(2000, 3, 15, 8, 0, 0));
project.Set(Prj.FinishDate, new DateTime(2000, 3, 21, 17, 0, 0));

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.IsManual, false);
task.Set(Tsk.Start, new DateTime(2000, 3, 15, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(4));

var assignment = project.ResourceAssignments.Add(task, project.Resources.Add("Resource"));
assignment.Set(Asn.Start, new DateTime(2000, 3, 15, 8, 0, 0));
assignment.Set(Asn.Work, task.Get(Tsk.Work));
assignment.Set(Asn.Finish, new DateTime(2000, 3, 19, 17, 0, 0));

// doit d'abord générer les données temporelles d'affectation de ressources
assignment.TimephasedDataFromTaskDuration(project.Get(Prj.Calendar));
Console.WriteLine(assignment.Get(Asn.Finish));

// diviser la tâche.
assignment.SplitTask(new DateTime(2000, 3, 16, 8, 0, 0), new DateTime(2000, 3, 17, 17, 0, 0), project.Get(Prj.Calendar));

// L'égalité des parties découpées est vérifiée par rapport au début, à la fin et à l'index des parties découpées.
var part1 = task.SplitParts[0];
var part2 = task.SplitParts[1];
Console.WriteLine("Split Part 1 Start {0} Finish {1}", part1.Start, part1.Finish);
Console.WriteLine("Split Part 2 Start {0} Finish {1}", part2.Start, part2.Finish);
Console.WriteLine("Are split parts equal: " + part1.Equals(part2));
```

### Voir aussi

* class [SplitPart](../)
* namespace [Aspose.Tasks](../../splitpart/)
* assembly [Aspose.Tasks](../../../)


