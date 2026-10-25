---
title: "SplitPart.Start"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété SplitPart. Obtient la date de début d'un SplitPart"
type: docs
weight: 20
url: /fr/net/aspose.tasks/splitpart/start/
---
## SplitPart.Start property

Obtient la date de début d'un SplitPart.

```csharp
public DateTime Start { get; }
```

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

* class [SplitPart](../)
* namespace [Aspose.Tasks](../../splitpart/)
* assembly [Aspose.Tasks](../../../)


