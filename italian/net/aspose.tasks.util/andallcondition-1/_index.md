---
title: "Classe AndAllConditionT"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Util.AndAllCondition1T. Applica l'AND logico a tutte le condizioni. Ad esempio cond1 AND cond2 AND cond3"
type: docs
weight: 2660
url: /it/net/aspose.tasks.util/andallcondition-1/
---
## AndAllCondition&lt;T&gt; class

Applica l'AND logico a tutte le condizioni. Per esempio: cond1 AND cond2 AND cond3...

```csharp
public class AndAllCondition<T> : ICondition<T>
```

| Parametro | Descrizione |
| --- | --- |
| T | Il tipo di oggetto a cui applicare l'interfaccia del metodo. |

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [AndAllCondition](andallcondition/)(List&lt;ICondition&lt;T&gt;&gt;) | Inizializza una nuova istanza della classe `AndAllCondition`. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Check](../../aspose.tasks.util/andallcondition-1/check/)(T) | Restituisce true se l'oggetto specificato soddisfa le condizioni. |

## Esempi

Mostra come utilizzare la condizione &lt;see cref=\"Aspose.Tasks.Util.AndAllCondition`1\" /&gt;.

```csharp
public void WorkWithAndAllCondition()
{
    var project = new Project(DataDir + "Project2.mpp");

    // raccogli tutti i task del progetto
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, coll, 0);

    var conditions = new List<ICondition<Task>>
                         {
                             // crea una condizione di filtro che filtra i task non nulli
                             new NotNullCondition(),

                             // crea una condizione di filtro che filtra i task di riepilogo
                             new SummaryCondition()
                         };

    // e unirli applicando la condizione <see cref=\"Aspose.Tasks.Util.AndAllCondition`1\" />
    var joinedCondition = new AndAllCondition<Task>(conditions);

    // applica la condizione ai task raccolti
    List<Task> collection = Filter(coll.Tasks, joinedCondition);
    Console.WriteLine("Filtered tasks: ");
    foreach (var task in collection)
    {
        Console.WriteLine("  Name: " + task.Get(Tsk.Name));

        // lavora con altre proprietà...
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

### Vedi anche

* interface [ICondition&lt;T&gt;](../icondition-1/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


