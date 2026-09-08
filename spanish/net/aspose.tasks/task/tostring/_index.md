---
title: "Task.ToString"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Task. Devuelve una representación corta en forma de cadena de una tarea. Los detalles exactos de la representación no están especificados y pueden cambiar."
type: docs
weight: 1420
url: /es/net/aspose.tasks/task/tostring/
---
## Task.ToString method

Devuelve una representación de cadena corta de una tarea. Los detalles exactos de la representación no están especificados y pueden cambiar.

```csharp
public override string ToString()
```

### Valor devuelto

cadena corta que representa el objeto tarea.

## Ejemplos

Muestra cómo ordenar tareas por nombre.

```csharp
public void SortTasksByName()
{
    var project = new Project(DataDir + "project-sort.mpp");
    var collector = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, collector, 0);
    List<Task> tasks = collector.Tasks;

    tasks.Sort(new TaskNameComparer());

    foreach (var task in tasks)
    {
        Console.WriteLine(task.ToString());
    }
}

private class TaskNameComparer : IComparer<Task>
{
    public int Compare(Task x, Task y)
    {
        if (x == null && y == null)
        {
            return 0;
        }

        if (x == null)
        {
            return -1;
        }

        if (y == null)
        {
            return 1;
        }

        if (string.IsNullOrEmpty(x.Get(Tsk.Name)))
        {
            return 1;
        }

        if (string.IsNullOrEmpty(y.Get(Tsk.Name)))
        {
            return -1;
        }

        return string.Compare(x.Get(Tsk.Name), y.Get(Tsk.Name), StringComparison.Ordinal);
    }
}
```

### Ver también

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


