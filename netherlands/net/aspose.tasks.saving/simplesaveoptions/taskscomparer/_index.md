---
title: "SimpleSaveOptions.TasksComparer"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "SimpleSaveOptions eigenschap. Haalt de vergelijker op of stelt deze in om taken te sorteren op de Gantt‑grafiek en de taakblad‑grafiek"
type: docs
weight: 20
url: /nl/net/aspose.tasks.saving/simplesaveoptions/taskscomparer/
---
## SimpleSaveOptions.TasksComparer property

Haalt op of stelt de comparer in om taken te sorteren op het Gantt‑diagram en het Task‑Sheet‑diagram.

```csharp
public IComparer<Task> TasksComparer { get; set; }
```

## Voorbeelden

Toont hoe je een comparer instelt om taken te sorteren op het Gantt-diagram en/of het Task Sheet-diagram.

```csharp
public void SortTasksByColumnInGanttChartExample()
{
    var project = new Project(DataDir + "Project2.mpp");
    SaveOptions options = new PdfSaveOptions
    {
        Timescale = Timescale.Months,
        TasksComparer = new TasksNameComparer()
    };
    project.Save(OutDir + "SortedByNames_out.pdf", options);

    options.TasksComparer = new TasksDurationComparer();
    project.Save(OutDir + "SortedByDurations_out.pdf", options);
}

private class TasksNameComparer : IComparer<Task>
{
    public int Compare(Task x, Task y)
    {
        // ReSharper disable once ConvertIfStatementToSwitchStatement
        // ReSharper disable once ConvertIfStatementToSwitchExpression
        if (x == null && y == null)
        {
            return 0;
        }

        if (x == null)
        {
            return -1;
        }

        return y == null ? 1 : string.Compare(x.Get(Tsk.Name), y.Get(Tsk.Name), StringComparison.Ordinal);
    }
}

private class TasksDurationComparer : IComparer<Task>
{
    public int Compare(Task x, Task y)
    {
        // ReSharper disable once ConvertIfStatementToSwitchStatement
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

        var durX = x.Get(Tsk.Duration);
        var durY = y.Get(Tsk.Duration);
        return durX.TimeSpan.CompareTo(durY.TimeSpan);
    }
}
```

### Zie ook

* class [Task](../../../aspose.tasks/task/)
* class [SimpleSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../simplesaveoptions/)
* assembly [Aspose.Tasks](../../../)


