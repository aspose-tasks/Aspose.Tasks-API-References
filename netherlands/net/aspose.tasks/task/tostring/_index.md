---
title: "Task.ToString"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Task-methode. Retourneert een korte tekenreeksrepresentatie van een taak. De exacte details van de representatie zijn niet gespecificeerd en kunnen wijzigen."
type: docs
weight: 1420
url: /nl/net/aspose.tasks/task/tostring/
---
## Task.ToString method

Retourneert een korte tekenreeksrepresentatie van een taak. De exacte details van de representatie zijn niet gespecificeerd en kunnen wijzigen.

```csharp
public override string ToString()
```

### Retourwaarde

korte tekenreeks die een taakobject representeert.

## Voorbeelden

Toont hoe taken gesorteerd kunnen worden op naam.

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

### Zie ook

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


