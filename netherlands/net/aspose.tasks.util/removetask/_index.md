---
title: "Klasse RemoveTask"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Util.RemoveTask klasse. Verwijdert de opgegeven taak uit een boom van taken"
type: docs
weight: 2760
url: /nl/net/aspose.tasks.util/removetask/
---
## RemoveTask class

Verwijdert de opgegeven taak uit een boom van taken.

```csharp
public class RemoveTask : ITreeAlgorithm<Task>
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [RemoveTask](removetask/)(Task) | Initialiseert een nieuw exemplaar van de `RemoveTask` klasse. |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [Alg](../../aspose.tasks.util/removetask/alg/)(Task, int) | Doe niets. |
| [PostAlg](../../aspose.tasks.util/removetask/postalg/)(Task, int) | Doe niets. |
| [PreAlg](../../aspose.tasks.util/removetask/prealg/)(Task, int) | Verwijdert de taak van de opgegeven bovenliggende taak. |

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

* interface [ITreeAlgorithm&lt;T&gt;](../itreealgorithm-1/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


