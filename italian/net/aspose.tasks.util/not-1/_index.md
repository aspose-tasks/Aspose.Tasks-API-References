---
title: "Classe NotT"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.Util.Not1T classe. Applica il NOT logico alla condizione specificata"
type: docs
weight: 2750
url: /it/net/aspose.tasks.util/not-1/
---
## Not&lt;T&gt; class

Applica il NOT logico alla condizione specificata.

```csharp
public class Not<T> : ICondition<T>
```

| Parametro | Descrizione |
| --- | --- |
| T | Il tipo di oggetto a cui applicare l'interfaccia del metodo. |

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [Not](not/)(ICondition&lt;T&gt;) | Inizializza una nuova istanza della classe `Not`. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Check](../../aspose.tasks.util/not-1/check/)(T) | Restituisce true se l'oggetto specificato soddisfa la condizione. |

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

* interface [ICondition&lt;T&gt;](../icondition-1/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


