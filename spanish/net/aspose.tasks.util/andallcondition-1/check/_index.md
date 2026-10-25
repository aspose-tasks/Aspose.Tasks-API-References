---
title: "AndAllCondition1.Check"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método AndAllCondition. Devuelve true si el objeto especificado cumple las condiciones"
type: docs
weight: 20
url: /es/net/aspose.tasks.util/andallcondition-1/check/
---
## AndAllCondition&lt;T&gt;.Check method

Devuelve true si el objeto especificado satisface las condiciones.

```csharp
public bool Check(T el)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| el | T | El objeto a comprobar. |

### Valor devuelto

Verdadero si el objeto cumple las condiciones.

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

* class [AndAllCondition&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../andallcondition-1/)
* assembly [Aspose.Tasks](../../../)


