---
title: "Clase NotT"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Util.Not1T. Aplica NOT lógico a la condición especificada"
type: docs
weight: 2750
url: /es/net/aspose.tasks.util/not-1/
---
## Not&lt;T&gt; class

Aplica NOT lógico a la condición especificada.

```csharp
public class Not<T> : ICondition<T>
```

| Parámetro | Descripción |
| --- | --- |
| T | El tipo de objeto al que aplicar la interfaz del método. |

## Constructores

| Nombre | Descripción |
| --- | --- |
| [Not](not/)(ICondition&lt;T&gt;) | Inicializa una nueva instancia de la clase `Not`. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Check](../../aspose.tasks.util/not-1/check/)(T) | Devuelve true si el objeto especificado satisface la condición. |

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

* interface [ICondition&lt;T&gt;](../icondition-1/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


