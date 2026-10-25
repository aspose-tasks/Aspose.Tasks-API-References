---
title: "Clase AndT"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Util.And1T. Aplica AND lógico a las condiciones especificadas"
type: docs
weight: 2670
url: /es/net/aspose.tasks.util/and-1/
---
## And&lt;T&gt; class

Aplica AND lógico a las condiciones especificadas.

```csharp
public class And<T> : ICondition<T>
```

| Parámetro | Descripción |
| --- | --- |
| T | El tipo de objeto al que aplicar la interfaz del método. |

## Constructores

| Nombre | Descripción |
| --- | --- |
| [And](and/)(ICondition&lt;T&gt;, ICondition&lt;T&gt;) | Inicializa una nueva instancia de la clase `And`. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Check](../../aspose.tasks.util/and-1/check/)(T) | Devuelve true si el objeto especificado satisface las condiciones. |

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

* interface [ICondition&lt;T&gt;](../icondition-1/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


