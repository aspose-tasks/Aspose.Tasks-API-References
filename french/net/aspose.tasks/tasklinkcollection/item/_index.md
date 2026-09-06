---
title: "TaskLinkCollection.Item"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété TaskLinkCollection. Retourne ou définit l'élément à l'index spécifié"
type: docs
weight: 20
url: /fr/net/aspose.tasks/tasklinkcollection/item/
---
## TaskLinkCollection indexer

Renvoie ou définit l'élément à l'index spécifié.

```csharp
public TaskLink this[int index] { get; set; }
```

| Paramètre | Description |
| --- | --- |
| index | L'index basé sur zéro de l'élément à obtenir ou définir. |

### Valeur de retour

l'élément à l'index spécifié.

## Exemples

Montre comment travailler avec des collections de liens de tâche.

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// obtenir les tâches
var task1 = project.RootTask.Children.GetById(1);
var task2 = project.RootTask.Children.GetById(2);
var task3 = project.RootTask.Children.GetById(3);
var task4 = project.RootTask.Children.GetById(4);
var task5 = project.RootTask.Children.GetById(5);

// lier les tâches
project.TaskLinks.Add(task1, task2);
project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart, project.GetDuration(1, TimeUnitType.Day));
project.TaskLinks.Add(task2, task5, TaskLinkType.FinishToStart, project.GetDuration(2, TimeUnitType.Day));

// imprimer les liens entre les tâches
Console.WriteLine("Print task links of " + project.TaskLinks.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Task links count: " + project.TaskLinks.Count);
foreach (var link in project.TaskLinks)
{
    Console.WriteLine("From ID = " + link.PredTask.Get(Tsk.Id) + " => To ID = " + link.SuccTask.Get(Tsk.Id));
    Console.WriteLine();
}

// modifier le lien par accès indexé
project.TaskLinks[0].LagFormat = TimeUnitType.Hour;

// supprimer tous les liens de tâche
List<TaskLink> taskLinks = project.TaskLinks.ToList();
foreach (var link in taskLinks)
{
    project.TaskLinks.Remove(link);
}
```

### Voir aussi

* class [TaskLink](../../tasklink/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)


