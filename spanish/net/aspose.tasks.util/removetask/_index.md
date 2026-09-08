---
title: "Clase RemoveTask"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Util.RemoveTask. Elimina la tarea especificada de un árbol de tareas"
type: docs
weight: 2760
url: /es/net/aspose.tasks.util/removetask/
---
## RemoveTask class

Elimina la tarea especificada de un árbol de tareas.

```csharp
public class RemoveTask : ITreeAlgorithm<Task>
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [RemoveTask](removetask/)(Task) | Inicializa una nueva instancia de la clase `RemoveTask`. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Alg](../../aspose.tasks.util/removetask/alg/)(Task, int) | No hacer nada. |
| [PostAlg](../../aspose.tasks.util/removetask/postalg/)(Task, int) | No hacer nada. |
| [PreAlg](../../aspose.tasks.util/removetask/prealg/)(Task, int) | Elimina la tarea de la tarea padre especificada. |

## Ejemplos

Muestra cómo usar el algoritmo basado en árbol &lt;see cref="Aspose.Tasks.Util.RemoveTask" /&gt;.

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

    // usar algoritmo basado en árbol para eliminar task1 del árbol
    var algorithm = new RemoveTask(task1);

    // aplicar el algoritmo al árbol de tareas
    TaskUtils.Apply(project.RootTask, algorithm, 0);

    // verificar los resultados
    tasks = new List<Task>(project.RootTask.SelectAllChildTasks());
    Console.WriteLine("Number of tasks after using the algorithm: " + tasks.Count);
    foreach (var task in project.RootTask.SelectAllChildTasks())
    {
        Console.WriteLine("Task Name: " + task.Get(Tsk.Name));
    }

    // ...
}
```

### Ver también

* interface [ITreeAlgorithm&lt;T&gt;](../itreealgorithm-1/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


