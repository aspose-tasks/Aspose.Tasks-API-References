---
title: "And1.And"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor de And. Inicializa una nueva instancia de la clase And"
type: docs
weight: 10
url: /es/net/aspose.tasks.util/and-1/and/
---
## And&lt;T&gt; constructor

Inicializa una nueva instancia de la clase [`And`](../).

```csharp
public And(ICondition<T> cond1, ICondition<T> cond2)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cond1 | ICondition`1 | Primera condición. |
| cond2 | ICondition`1 | Segunda condición. |

## Ejemplos

Muestra cómo usar la condición &lt;see cref=\"Aspose.Tasks.Util.And`1\" /&gt;.

```csharp
public void WorkWithAnd()
{
    var project = new Project(DataDir + "Project2.mpp");

    // recopila todas las tareas del proyecto
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, coll, 0);

    // crear una condición de filtro que filtre las tareas resumen
    var condition1 = new SummaryCondition();

    // crear una condición de filtro que filtre las tareas no nulas
    var condition2 = new NotNullCondition();

    // y únelas aplicando la condición <see cref=\"Aspose.Tasks.Util.And`1\" />
    var joinedCondition = new And<Task>(condition1, condition2);

    // aplicar la condición a las tareas recopiladas
    List<Task> collection = Filter(coll.Tasks, joinedCondition);
    Console.WriteLine("Filtered tasks: ");
    foreach (var task in collection)
    {
        Console.WriteLine(" Name: " + task.Get(Tsk.Name));

        // trabajar con otras propiedades...
    }

    // ...
}

private static List<T> Filter<T>(IEnumerable<T> array, ICondition<T> cond)
{
    var result = new List<T>();

    foreach (var item in array)
    {
        if (cond.Check(item))
        {
            result.Add(item);
        }
    }

    return result;
}

private class NotNullCondition : ICondition<Task>
{
    public bool Check(Task el)
    {
        return !el.Get(Tsk.IsNull).Value;
    }
}

private class SummaryCondition : ICondition<Task>
{
    public bool Check(Task el)
    {
        return el.Get(Tsk.IsSummary);
    }
}
```

### Ver también

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [And&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../and-1/)
* assembly [Aspose.Tasks](../../../)


