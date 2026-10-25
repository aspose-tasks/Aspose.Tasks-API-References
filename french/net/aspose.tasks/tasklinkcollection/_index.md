---
title: "Classe TaskLinkCollection"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.TaskLinkCollection. Représente une collection d'objets Task"
type: docs
weight: 2420
url: /fr/net/aspose.tasks/tasklinkcollection/
---
## TaskLinkCollection class

Représente une collection d'objets [`Task`](../task/).

```csharp
public class TaskLinkCollection : IList<TaskLink>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../aspose.tasks/tasklinkcollection/count/) { get; } | Obtient le nombre d'objets contenus dans cet objet `TaskLinkCollection`. |
| [Item](../../aspose.tasks/tasklinkcollection/item/) { get; set; } | Renvoie ou définit l'élément à l'index spécifié. |
| [ParentProject](../../aspose.tasks/tasklinkcollection/parentproject/) { get; } | Obtient le projet parent de l'objet ResourceAssignmentCollection. projet parent [`Project`](../project/) pour cet objet. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add_3)(TaskLink) | Ceci est l'implémentation factice de la méthode Add de ICollection, qui ne lance que NotSupportedException |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add)(Task, Task) | Renvoie une instance de Finish-Start [`TaskLink`](../tasklink/) qui a été ajoutée à l'objet TaskLinkCollection. |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add_1)(Task, Task, TaskLinkType) | Renvoie une instance de [`TaskLink`](../tasklink/) qui a été ajoutée à l'objet TaskLinkCollection. |
| [Add](../../aspose.tasks/tasklinkcollection/add/#add_2)(Task, Task, TaskLinkType, Duration) | Renvoie une instance de [`TaskLink`](../tasklink/) qui a été ajoutée à l'objet TaskLinkCollection. |
| [GetEnumerator](../../aspose.tasks/tasklinkcollection/getenumerator/)() | Renvoie un énumérateur pour cette collection. |
| [Remove](../../aspose.tasks/tasklinkcollection/remove/)(TaskLink) | Supprime le lien de tâche d'un projet. |
| [ToList](../../aspose.tasks/tasklinkcollection/tolist/)() | Convertit l'objet TaskLinkCollection en une liste d'objets [`TaskLink`](../tasklink/). |

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

* class [TaskLink](../tasklink/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


