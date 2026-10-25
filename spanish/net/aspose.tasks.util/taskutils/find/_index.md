---
title: "TaskUtils.Find"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método TaskUtils. Encuentra una tarea que cumpla la condición en un árbol de tareas"
type: docs
weight: 30
url: /es/net/aspose.tasks.util/taskutils/find/
---
## TaskUtils.Find method

Encuentra una tarea que cumple la condición en un árbol de tareas.

```csharp
public static Task Find(Task root, ICondition<Task> cond)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| root | Tarea | Raíz del árbol. |
| cond | ICondition`1 | Condición aplicada. |

### Valor devuelto

Tarea si se encontró, de lo contrario null.

## Ejemplos

Muestra cómo usar &lt;see cref="Aspose.Tasks.Util.TaskUtils.Find" /&gt; método.

```csharp
public void WorkWithFind()
{
    var project = new Project(DataDir + "Project2.mpp");

    // construye un nuevo árbol de tareas que cumplen la condición 
    var task = TaskUtils.Filter(project.RootTask, new FindByName("Task8"));

    // recopila tareas de un árbol
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(task, coll, 0);

    // itera sobre una lista simple de tareas 
    // cuyas duraciones son mayores o iguales a 2 días laborables
    foreach (var collTask in coll.Tasks)
    {
        Console.WriteLine("Name: " + collTask.Get(Tsk.Name) + "Duration: " + collTask.Get(Tsk.Duration).TimeSpan);
    }
}

private class FindByName : ICondition<Task>
{
    private readonly string name;

    public FindByName(string name)
    {
        this.name = name;
    }

    /// <summary>
    /// Devuelve verdadero si el objeto especificado cumple las condiciones.
    /// </summary>
    /// <param name=\"el\">El objeto a verificar.</param>
    /// <returns>Verdadero si el objeto cumple las condiciones.</returns>
    /// <inheritdoc />
    public bool Check(Task el)
    {
        return el.Get(Tsk.Name) == this.name;
    }
}
```

### Ver también

* class [Task](../../../aspose.tasks/task/)
* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


