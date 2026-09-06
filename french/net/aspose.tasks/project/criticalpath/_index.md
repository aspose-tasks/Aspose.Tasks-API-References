---
title: "Project.CriticalPath"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété du projet. Obtient une collection qui contient une liste de tâches critiques qui composent le Chemin critique de ce projet. Il s'agit d'une opération On où n est le nombre de tâches dans le projet"
type: docs
weight: 180
url: /fr/net/aspose.tasks/project/criticalpath/
---
## Project.CriticalPath property

Obtient une collection qui contient une liste de tâches Critical qui composent le chemin critique de ce projet. Il s'agit d'une opération O(n), où n est le nombre de tâches du projet.

```csharp
public TaskCollection CriticalPath { get; }
```

### Valeur de retour

une collection qui représente une liste de toutes les tâches critiques.

## Exemples

Montre comment calculer le chemin critique du projet.

```csharp
var project = new Project()
{
    CalculationMode = CalculationMode.Automatic
};

var subtask1 = project.RootTask.Children.Add("1");
var subtask2 = project.RootTask.Children.Add("2");
project.TaskLinks.Add(subtask1, subtask2, TaskLinkType.FinishToStart);

project.RootTask.Children.Add("3");

// Affiche le chemin critique maintenant
foreach (var task in project.CriticalPath)
{
    Console.WriteLine(task.Get(Tsk.Id) + "  " + task.Get(Tsk.Name));
    Console.WriteLine(task.Get(Tsk.Start));
    Console.WriteLine(task.Get(Tsk.Finish) + "\n");
}
```

### Voir aussi

* class [TaskCollection](../../taskcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


