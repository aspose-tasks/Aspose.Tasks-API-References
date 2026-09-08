---
title: "TaskUtils.Filter"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método TaskUtils. Construye un nuevo árbol de tareas que cumplen la condición"
type: docs
weight: 20
url: /es/net/aspose.tasks.util/taskutils/filter/
---
## TaskUtils.Filter method

Construye un nuevo árbol de tareas que cumplen la condición.

```csharp
public static Task Filter(Task root, ICondition<Task> cond)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| root | Tarea | Raíz del árbol. |
| cond | ICondition`1 | Condición aplicada. |

### Valor devuelto

Raíz de un nuevo árbol.

## Ejemplos

Muestra cómo trabajar con una condición.

```csharp
[Test] //ExSkip
public void WorkWithFilter()
{
    var project = new Project(DataDir + "Project2.mpp");

    // construye un nuevo árbol de tareas que cumplen la condición 
    var task = TaskUtils.Filter(project.RootTask, new FilterByDuration(2));

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

private class FilterByDuration : ICondition<Task>
{
    private readonly int days;

    public FilterByDuration(int days)
    {
        this.days = days;
    }

    /// <summary>
    /// Devuelve verdadero si el objeto especificado cumple las condiciones.
    /// </summary>
    /// <param name=\"el\">El objeto a verificar.</param>
    /// <returns>Verdadero si el objeto cumple las condiciones.</returns>
    /// <inheritdoc />
    public bool Check(Task el)
    {
        return el.Get(Tsk.Duration).TimeSpan >= TimeSpan.FromHours(this.days * 8);
    }
}
```

### Ver también

* class [Task](../../../aspose.tasks/task/)
* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


