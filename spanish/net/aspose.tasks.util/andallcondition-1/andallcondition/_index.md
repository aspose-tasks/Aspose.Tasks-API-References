---
title: "AndAllCondition1.AndAllCondition"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor AndAllCondition. Inicializa una nueva instancia de la clase AndAllCondition"
type: docs
weight: 10
url: /es/net/aspose.tasks.util/andallcondition-1/andallcondition/
---
## AndAllCondition&lt;T&gt; constructor

Inicializa una nueva instancia de la clase [`AndAllCondition`](../).

```csharp
public AndAllCondition(List<ICondition<T>> conditions)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| condiciones | List`1 | La lista de condiciones. |

## Ejemplos

Muestra cómo usar la condición &lt;see cref=\"Aspose.Tasks.Util.AndAllCondition`1\" /&gt;.

```csharp
public void WorkWithAndAllCondition()
{
    var project = new Project(DataDir + "Project2.mpp");

    // recopila todas las tareas del proyecto
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, coll, 0);

    var conditions = new List<ICondition<Task>>
                         {
                             // crear una condición de filtro que filtre las tareas no nulas
                             new NotNullCondition(),

                             // crear una condición de filtro que filtre las tareas resumen
                             new SummaryCondition()
                         };

    // y únalos aplicando la condición <see cref=\"Aspose.Tasks.Util.AndAllCondition`1\" />
    var joinedCondition = new AndAllCondition<Task>(conditions);

    // aplicar la condición a las tareas recopiladas
    List<Task> collection = Filter(coll.Tasks, joinedCondition);
    Console.WriteLine("Filtered tasks: ");
    foreach (var task in collection)
    {
        Console.WriteLine("  Name: " + task.Get(Tsk.Name));

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
* class [AndAllCondition&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../andallcondition-1/)
* assembly [Aspose.Tasks](../../../)


