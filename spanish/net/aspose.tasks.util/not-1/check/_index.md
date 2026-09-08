---
title: "Not1.Check"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Not. Devuelve true si el objeto especificado cumple la condición"
type: docs
weight: 20
url: /es/net/aspose.tasks.util/not-1/check/
---
## Not&lt;T&gt;.Check method

Devuelve true si el objeto especificado satisface la condición.

```csharp
public bool Check(T el)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| el | T | El objeto a comprobar. |

### Valor devuelto

Verdadero si el objeto cumple la condición.

## Ejemplos

Muestra cómo usar la condición &lt;see cref=\"Aspose.Tasks.Util.Not`1\" /&gt;.

```csharp
public void WorkWithNot()
{
    var project = new Project(DataDir + "Project2.mpp");

    // recopila todas las tareas del proyecto
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, coll, 0);

    // crear una condición de filtro
    var filter = new NullCondition();

    // y revierte aplicando la condición <see cref=\"Aspose.Tasks.Util.Not`1\" />
    var condition = new Not<Task>(filter);

    // aplicar la condición a las tareas recopiladas
    List<Task> collection = Filter(coll.Tasks, condition);
    foreach (var task in collection)
    {
        Console.WriteLine("Name: " + task.Get(Tsk.Name));

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

private class NullCondition : ICondition<Task>
{
    public bool Check(Task el)
    {
        return el.Get(Tsk.IsNull).Value;
    }
}
```

### Ver también

* class [Not&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../not-1/)
* assembly [Aspose.Tasks](../../../)


