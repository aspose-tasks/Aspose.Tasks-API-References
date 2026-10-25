---
title: "TaskUtils.Find"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo TaskUtils. Trova un'attività che soddisfa la condizione in un albero di attività"
type: docs
weight: 30
url: /it/net/aspose.tasks.util/taskutils/find/
---
## TaskUtils.Find method

Trova un task che soddisfa la condizione in un albero di task.

```csharp
public static Task Find(Task root, ICondition<Task> cond)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| root | Attività | Radice dell'albero. |
| cond | ICondition`1 | Condizione applicata. |

### Valore di ritorno

Task se l'attività è stata trovata, altrimenti null.

## Esempi

Mostra come utilizzare &lt;see cref="Aspose.Tasks.Util.TaskUtils.Find" /&gt; metodo.

```csharp
public void WorkWithFind()
{
    var project = new Project(DataDir + "Project2.mpp");

    // costruisce un nuovo albero di attività che soddisfano la condizione 
    var task = TaskUtils.Filter(project.RootTask, new FindByName("Task8"));

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

private class FindByName : ICondition<Task>
{
    private readonly string name;

    public FindByName(string name)
    {
        this.name = name;
    }

    /// <summary>
    /// Restituisce true se l'oggetto specificato soddisfa le condizioni.
    /// </summary>
    /// <param name=\"el\">L'oggetto da verificare.</param>
    /// <returns>True se l'oggetto soddisfa le condizioni.</returns>
    /// <inheritdoc />
    public bool Check(Task el)
    {
        return el.Get(Tsk.Name) == this.name;
    }
}
```

### Vedi anche

* class [Task](../../../aspose.tasks/task/)
* interface [ICondition&lt;T&gt;](../../icondition-1/)
* class [TaskUtils](../)
* namespace [Aspose.Tasks.Util](../../taskutils/)
* assembly [Aspose.Tasks](../../../)


