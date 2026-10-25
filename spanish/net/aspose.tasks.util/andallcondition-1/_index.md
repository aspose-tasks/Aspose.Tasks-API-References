---
title: "Clase AndAllConditionT"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Util.AndAllCondition1T. Aplica AND lógico a todas las condiciones. Por ejemplo cond1 AND cond2 AND cond3"
type: docs
weight: 2660
url: /es/net/aspose.tasks.util/andallcondition-1/
---
## AndAllCondition&lt;T&gt; class

Aplica AND lógico a todas las condiciones. Por ejemplo: cond1 AND cond2 AND cond3...

```csharp
public class AndAllCondition<T> : ICondition<T>
```

| Parámetro | Descripción |
| --- | --- |
| T | El tipo de objeto al que aplicar la interfaz del método. |

## Constructores

| Nombre | Descripción |
| --- | --- |
| [AndAllCondition](andallcondition/)(List&lt;ICondition&lt;T&gt;&gt;) | Inicializa una nueva instancia de la clase `AndAllCondition`. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Check](../../aspose.tasks.util/andallcondition-1/check/)(T) | Devuelve true si el objeto especificado satisface las condiciones. |

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

* interface [ICondition&lt;T&gt;](../icondition-1/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


