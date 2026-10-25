---
title: "Not1.Check"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Not. Restituisce true se l'oggetto specificato soddisfa la condizione"
type: docs
weight: 20
url: /it/net/aspose.tasks.util/not-1/check/
---
## Not&lt;T&gt;.Check method

Restituisce true se l'oggetto specificato soddisfa la condizione.

```csharp
public bool Check(T el)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| el | T | L'oggetto da controllare. |

### Valore di ritorno

Vero se l'oggetto soddisfa la condizione.

## Esempi

Mostra come utilizzare la condizione &lt;see cref="Aspose.Tasks.Util.Not`1" /&gt;.

```csharp
public void WorkWithNot()
{
    var project = new Project(DataDir + "Project2.mpp");

    // raccogli tutti i task del progetto
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, coll, 0);

    // crea una condizione di filtro
    var filter = new NullCondition();

    // e inverti applicando la condizione <see cref="Aspose.Tasks.Util.Not`1" />
    var condition = new Not<Task>(filter);

    // applica la condizione ai task raccolti
    List<Task> collection = Filter(coll.Tasks, condition);
    foreach (var task in collection)
    {
        Console.WriteLine("Name: " + task.Get(Tsk.Name));

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

private class NullCondition : ICondition<Task>
{
    public bool Check(Task el)
    {
        return el.Get(Tsk.IsNull).Value;
    }
}
```

### Vedi anche

* class [Not&lt;T&gt;](../)
* namespace [Aspose.Tasks.Util](../../not-1/)
* assembly [Aspose.Tasks](../../../)


