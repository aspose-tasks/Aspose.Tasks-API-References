---
title: "RemoveTask.Alg"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método RemoveTask. No hace nada"
type: docs
weight: 20
url: /es/net/aspose.tasks.util/removetask/alg/
---
## RemoveTask.Alg method

No hacer nada.

```csharp
public void Alg(Task el, int level)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| el | Tarea | Objeto a procesar. |
| nivel | Int32 | Nivel del nodo del árbol. |

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

* class [Task](../../../aspose.tasks/task/)
* class [RemoveTask](../)
* namespace [Aspose.Tasks.Util](../../removetask/)
* assembly [Aspose.Tasks](../../../)


