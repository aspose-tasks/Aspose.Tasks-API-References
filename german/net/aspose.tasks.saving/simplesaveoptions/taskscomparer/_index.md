---
title: "SimpleSaveOptions.TasksComparer"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "SimpleSaveOptions-Eigenschaft. Gibt den Comparer zurück oder legt ihn fest, um Aufgaben im Gantt-Diagramm und im Aufgabenblatt-Diagramm zu sortieren."
type: docs
weight: 20
url: /de/net/aspose.tasks.saving/simplesaveoptions/taskscomparer/
---
## SimpleSaveOptions.TasksComparer property

Liest oder setzt den Vergleicher, um Aufgaben im Gantt‑Diagramm und im Task‑Sheet‑Diagramm zu sortieren.

```csharp
public IComparer<Task> TasksComparer { get; set; }
```

## Beispiele

Zeigt, wie ein Comparer festgelegt wird, um Aufgaben im Gantt-Diagramm und/oder im Aufgabenblatt-Diagramm zu sortieren.

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

### Siehe auch

* class [Task](../../../aspose.tasks/task/)
* class [SimpleSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../simplesaveoptions/)
* assembly [Aspose.Tasks](../../../)


