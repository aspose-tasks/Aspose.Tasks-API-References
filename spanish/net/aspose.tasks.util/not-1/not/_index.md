---
title: "Not1.Not"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor Not. Inicializa una nueva instancia de la clase Not"
type: docs
weight: 10
url: /es/net/aspose.tasks.util/not-1/not/
---
## Not&lt;T&gt; constructor

Inicializa una nueva instancia de la clase [`Not`](../).

```csharp
public Not(ICondition<T> condition)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| condición | ICondition`1 | Condición especificada. |

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

* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [Not&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../not-1/)
* assembly [Aspose.Tasks](../../../)


