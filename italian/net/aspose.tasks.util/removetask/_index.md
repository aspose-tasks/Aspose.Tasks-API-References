---
title: "Classe RemoveTask"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Util.RemoveTask. Rimuove l'attività specificata da un albero di attività"
type: docs
weight: 2760
url: /it/net/aspose.tasks.util/removetask/
---
## RemoveTask class

Rimuove l'attività specificata da un albero di attività.

```csharp
public class RemoveTask : ITreeAlgorithm<Task>
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [RemoveTask](removetask/)(Task) | Inizializza una nuova istanza della classe `RemoveTask`. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Alg](../../aspose.tasks.util/removetask/alg/)(Task, int) | Non fare nulla. |
| [PostAlg](../../aspose.tasks.util/removetask/postalg/)(Task, int) | Non fare nulla. |
| [PreAlg](../../aspose.tasks.util/removetask/prealg/)(Task, int) | Rimuove l'attività dall'attività genitore specificata. |

## Esempi

Mostra come utilizzare l'algoritmo basato su albero &lt;see cref="Aspose.Tasks.Util.RemoveTask" /&gt;.

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

    // utilizza l'algoritmo basato su albero per eliminare task1 dall'albero
    var algorithm = new RemoveTask(task1);

    // applica l'algoritmo all'albero delle attività
    TaskUtils.Apply(project.RootTask, algorithm, 0);

    // controlla i risultati
    tasks = new List<Task>(project.RootTask.SelectAllChildTasks());
    Console.WriteLine("Number of tasks after using the algorithm: " + tasks.Count);
    foreach (var task in project.RootTask.SelectAllChildTasks())
    {
        Console.WriteLine("Task Name: " + task.Get(Tsk.Name));
    }

    // ...
}
```

### Vedi anche

* interface [ITreeAlgorithm&lt;T&gt;](../itreealgorithm-1/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


