---
title: "TaskLinkCollection.ToList"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode TaskLinkCollection. Convertit l'objet TaskLinkCollection en une liste d'objets TaskLink"
type: docs
weight: 70
url: /fr/net/aspose.tasks/tasklinkcollection/tolist/
---
## TaskLinkCollection.ToList method

Convertit l'objet TaskLinkCollection en une liste d'objets [`TaskLink`](../../tasklink/).

```csharp
public List<TaskLink> ToList()
```

### Valeur de retour

Liste d'objets [`TaskLink`](../../tasklink/).

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


