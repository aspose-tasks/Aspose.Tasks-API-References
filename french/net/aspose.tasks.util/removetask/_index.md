---
title: "Classe RemoveTask"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.Util.RemoveTask. Supprime la tâche spécifiée d'un arbre de tâches"
type: docs
weight: 2760
url: /fr/net/aspose.tasks.util/removetask/
---
## RemoveTask class

Supprime la tâche spécifiée d'un arbre de tâches.

```csharp
public class RemoveTask : ITreeAlgorithm<Task>
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [RemoveTask](removetask/)(Task) | Initialise une nouvelle instance de la classe `RemoveTask`. |

## Méthodes

| Nom | Description |
| --- | --- |
| [Alg](../../aspose.tasks.util/removetask/alg/)(Task, int) | Ne rien faire. |
| [PostAlg](../../aspose.tasks.util/removetask/postalg/)(Task, int) | Ne rien faire. |
| [PreAlg](../../aspose.tasks.util/removetask/prealg/)(Task, int) | Supprime la tâche du parent spécifié. |

## Exemples

Montre comment utiliser l'algorithme basé sur l'arbre &lt;see cref=\"Aspose.Tasks.Util.RemoveTask\" /&gt;.

```csharp
public void WorkWithRemoveTask()
{
    var project = new Project(DataDir + "Project1.mpp");
    var task1 = project.RootTask.Children.Add("1");
    var task2 = project.RootTask.Children.Add("2");
    var task3 = project.RootTask.Children.Add("3");
    var task4 = project.RootTask.Children.Add("4");

    List<Task> tasks = new List<Task>(project.RootTask.SelectAllChildTasks());
    Console.WriteLine("Number of tasks before using the algorithm: " + tasks.Count);
    foreach (var task in project.RootTask.SelectAllChildTasks())
    {
        Console.WriteLine("Task Name: " + task.Get(Tsk.Name));
    }

    Console.WriteLine();

    // utiliser l'algorithme basé sur l'arbre pour supprimer task1 de l'arbre
    var algorithm = new RemoveTask(task1);

    // appliquer l'algorithme à l'arbre des tâches
    TaskUtils.Apply(project.RootTask, algorithm, 0);

    // vérifier les résultats
    tasks = new List<Task>(project.RootTask.SelectAllChildTasks());
    Console.WriteLine("Number of tasks after using the algorithm: " + tasks.Count);
    foreach (var task in project.RootTask.SelectAllChildTasks())
    {
        Console.WriteLine("Task Name: " + task.Get(Tsk.Name));
    }

    // ...
}
```

### Voir aussi

* interface [ITreeAlgorithm&lt;T&gt;](../itreealgorithm-1/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


