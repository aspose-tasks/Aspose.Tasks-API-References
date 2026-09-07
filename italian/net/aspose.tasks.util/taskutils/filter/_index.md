---
title: "TaskUtils.Filter"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo TaskUtils. Costruisce un nuovo albero di attività che soddisfano la condizione"
type: docs
weight: 20
url: /it/net/aspose.tasks.util/taskutils/filter/
---
## TaskUtils.Filter method

Costruisce un nuovo albero di task che soddisfano la condizione.

```csharp
public static Task Filter(Task root, ICondition<Task> cond)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| root | Attività | Radice dell'albero. |
| cond | ICondition`1 | Condizione applicata. |

### Valore di ritorno

Radice di un nuovo albero.

## Esempi

Mostra come lavorare con una condizione.

```csharp
[Test] //ExSkip
public void WorkWithFilter()
{
    var project = new Project(DataDir + "Project2.mpp");

    // costruisce un nuovo albero di attività che soddisfano la condizione 
    var task = TaskUtils.Filter(project.RootTask, new FilterByDuration(2));

    // raccogli attività da un albero
    var coll = new ChildTasksCollector();
    TaskUtils.Apply(task, coll, 0);

    // itera su un semplice elenco di attività 
    // le cui durate sono maggiori o uguali a 2 giorni lavorativi
    foreach (var collTask in coll.Tasks)
    {
        Console.WriteLine("Name: " + collTask.Get(Tsk.Name) + "Duration: " + collTask.Get(Tsk.Duration).TimeSpan);
    }
}

private class FilterByDuration : ICondition<Task>
{
    private readonly int days;

    public FilterByDuration(int days)
    {
        this.days = days;
    }

    /// <summary>
    /// Restituisce true se l'oggetto specificato soddisfa le condizioni.
    /// </summary>
    /// <param name=\"el\">L'oggetto da verificare.</param>
    /// <returns>True se l'oggetto soddisfa le condizioni.</returns>
    /// <inheritdoc />
    public bool Check(Task el)
    {
        return el.Get(Tsk.Duration).TimeSpan >= TimeSpan.FromHours(this.days * 8);
    }
}
```

### Vedi anche

* class [Task](../../../aspose.tasks/task/)
* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


