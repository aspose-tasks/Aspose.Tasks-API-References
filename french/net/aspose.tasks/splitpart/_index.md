---
title: "Classe SplitPart"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.SplitPart. Représente une portion de tâche. Le SplitPart est un membre de la collection SplitParts des tâches."
type: docs
weight: 2290
url: /fr/net/aspose.tasks/splitpart/
---
## SplitPart class

Représente une portion de tâche. Le SplitPart est un membre de la collection SplitParts de la tâche.

```csharp
public class SplitPart
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Finish](../../aspose.tasks/splitpart/finish/) { get; } | Obtient la date de fin d'un SplitPart. |
| [Start](../../aspose.tasks/splitpart/start/) { get; } | Obtient la date de début d'un SplitPart. |

## Méthodes

| Nom | Description |
| --- | --- |
| override [Equals](../../aspose.tasks/splitpart/equals/)(object) | Compare deux parties découpées. |
| override [GetHashCode](../../aspose.tasks/splitpart/gethashcode/)() | Renvoie une valeur de code de hachage pour l'instance de la classe `SplitPart`. |

## Exemples

Montre comment travailler avec les parties découpées d'une tâche découpée.

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

// itérer sur les parties découpées
Console.WriteLine("Number of split parts: " + task.SplitParts.Count);
foreach (var splitPart in task.SplitParts)
{
    Console.WriteLine("  Split Part Start: " + splitPart.Start);
    Console.WriteLine("  Split Part Finish: " + splitPart.Finish);
    Console.WriteLine();
}
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


