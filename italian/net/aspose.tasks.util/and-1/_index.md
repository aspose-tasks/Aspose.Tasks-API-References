---
title: "Classe AndT"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Util.And1T. Applica l'AND logico alle condizioni specificate"
type: docs
weight: 2670
url: /it/net/aspose.tasks.util/and-1/
---
## And&lt;T&gt; class

Applica l'AND logico alle condizioni specificate.

```csharp
public class And<T> : ICondition<T>
```

| Parametro | Descrizione |
| --- | --- |
| T | Il tipo di oggetto a cui applicare l'interfaccia del metodo. |

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [And](and/)(ICondition&lt;T&gt;, ICondition&lt;T&gt;) | Inizializza una nuova istanza della classe `And`. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Check](../../aspose.tasks.util/and-1/check/)(T) | Restituisce true se l'oggetto specificato soddisfa le condizioni. |

## Esempi

Mostra come utilizzare la condizione &lt;see cref="Aspose.Tasks.Util.And`1" /&gt;.

```csharp
public void WorkWithAnd()
{
    var project = new Project(DataDir + "Project2.mpp");

    // raccogli tutti i task del progetto
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, coll, 0);

    // crea una condizione di filtro che filtra i task di riepilogo
    var condition1 = new SummaryCondition();

    // crea una condizione di filtro che filtra i task non nulli
    var condition2 = new NotNullCondition();

    // e uniscili applicando la condizione <see cref="Aspose.Tasks.Util.And`1" />
    var joinedCondition = new And<Task>(condition1, condition2);

    // applica la condizione ai task raccolti
    List<Task> collection = Filter(coll.Tasks, joinedCondition);
    Console.WriteLine("Filtered tasks: ");
    foreach (var task in collection)
    {
        Console.WriteLine(" Name: " + task.Get(Tsk.Name));

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


