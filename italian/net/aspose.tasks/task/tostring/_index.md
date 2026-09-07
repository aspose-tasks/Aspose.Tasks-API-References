---
title: "Task.ToString"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Task. Restituisce una breve rappresentazione testuale di un task. I dettagli esatti della rappresentazione non sono specificati e sono soggetti a modifiche"
type: docs
weight: 1420
url: /it/net/aspose.tasks/task/tostring/
---
## Task.ToString method

Restituisce una breve rappresentazione stringa di un'attività. I dettagli esatti della rappresentazione non sono specificati e possono cambiare.

```csharp
public override string ToString()
```

### Valore di ritorno

breve stringa che rappresenta l'oggetto task.

## Esempi

Mostra come ordinare i task per nome.

```csharp
public void SortTasksByName()
{
    var project = new Project(DataDir + "project-sort.mpp");
    var collector = new ChildTasksCollector();
    TaskUtils.Apply(project.RootTask, collector, 0);
    List<Task> tasks = collector.Tasks;

    tasks.Sort(new TaskNameComparer());

    foreach (var task in tasks)
    {
        Console.WriteLine(task.ToString());
    }
}

private class TaskNameComparer : IComparer<Task>
{
    public int Compare(Task x, Task y)
    {
        if (x == null && y == null)
        {
            return 0;
        }

        if (x == null)
        {
            return -1;
        }

        if (y == null)
        {
            return 1;
        }

        if (string.IsNullOrEmpty(x.Get(Tsk.Name)))
        {
            return 1;
        }

        if (string.IsNullOrEmpty(y.Get(Tsk.Name)))
        {
            return -1;
        }

        return string.Compare(x.Get(Tsk.Name), y.Get(Tsk.Name), StringComparison.Ordinal);
    }
}
```

### Vedi anche

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


