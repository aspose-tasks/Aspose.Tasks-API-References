---
title: "RemoveTask.RemoveTask"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Constructeur RemoveTask. Initialise une nouvelle instance de la classe RemoveTask"
type: docs
weight: 10
url: /fr/net/aspose.tasks.util/removetask/removetask/
---
## RemoveTask constructor

Initialise une nouvelle instance de la classe [`RemoveTask`](../).

```csharp
public RemoveTask(Task task)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| tâche | Tâche | Tâche à supprimer. |

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

* class [Task](../../../aspose.tasks/task/)
* class [RemoveTask](../)
* namespace [Aspose.Tasks.Util](../../removetask/)
* assembly [Aspose.Tasks](../../../)


