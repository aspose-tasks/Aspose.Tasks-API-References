---
title: "And1.Check"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método And. Devuelve verdadero si el objeto especificado cumple las condiciones"
type: docs
weight: 20
url: /es/net/aspose.tasks.util/and-1/check/
---
## And&lt;T&gt;.Check method

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

* class [And&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../and-1/)
* assembly [Aspose.Tasks](../../../)


