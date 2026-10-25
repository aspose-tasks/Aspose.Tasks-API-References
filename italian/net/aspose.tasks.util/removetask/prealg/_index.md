---
title: "RemoveTask.PreAlg"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo RemoveTask. Rimuove il compito dal compito genitore specificato"
type: docs
weight: 40
url: /it/net/aspose.tasks.util/removetask/prealg/
---
## RemoveTask.PreAlg method

Rimuove l'attività dall'attività genitore specificata.

```csharp
public void PreAlg(Task el, int level)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| el | Attività | Compito genitore. |
| livello | Int32 | Livello del nodo dell'albero. |

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

* class [Task](../../../aspose.tasks/task/)
* class [RemoveTask](../)
* namespace [Aspose.Tasks.Util](../../removetask/)
* assembly [Aspose.Tasks](../../../)


