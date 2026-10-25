---
title: "AndAllCondition1.Check"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo AndAllCondition. Restituisce true se l'oggetto specificato soddisfa le condizioni"
type: docs
weight: 20
url: /it/net/aspose.tasks.util/andallcondition-1/check/
---
## AndAllCondition&lt;T&gt;.Check method

Restituisce true se l'oggetto specificato soddisfa le condizioni.

```csharp
public bool Check(T el)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| el | T | L'oggetto da controllare. |

### Valore di ritorno

Vero se l'oggetto soddisfa le condizioni.

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

* class [AndAllCondition&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../andallcondition-1/)
* assembly [Aspose.Tasks](../../../)


