---
title: "RemoveTask.PostAlg"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "RemoveTask-methode. Doe niets"
type: docs
weight: 30
url: /nl/net/aspose.tasks.util/removetask/postalg/
---
## RemoveTask.PostAlg method

Doe niets.

```csharp
public void PostAlg(Task el, int level)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| el | Taak | Object om te verwerken. |
| niveau | Int32 | Boomknoopniveau. |

## Voorbeelden

Toont hoe je &lt;see cref="Aspose.Tasks.Util.RemoveTask" /&gt; boomgebaseerd algoritme gebruikt.

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

    // Gebruik een boomgebaseerd algoritme om task1 uit de boom te verwijderen
    var algorithm = new RemoveTask(task1);

    // Pas het algoritme toe op de takenboom
    TaskUtils.Apply(project.RootTask, algorithm, 0);

    // Controleer de resultaten
    tasks = new List<Task>(project.RootTask.SelectAllChildTasks());
    Console.WriteLine("Number of tasks after using the algorithm: " + tasks.Count);
    foreach (var task in project.RootTask.SelectAllChildTasks())
    {
        Console.WriteLine("Task Name: " + task.Get(Tsk.Name));
    }

    // ...
}
```

### Zie ook

* class [Task](../../../aspose.tasks/task/)
* class [RemoveTask](../)
* namespace [Aspose.Tasks.Util](../../removetask/)
* assembly [Aspose.Tasks](../../../)


