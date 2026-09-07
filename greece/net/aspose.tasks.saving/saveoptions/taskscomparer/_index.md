---
title: "TasksComparer"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Λαμβάνει ή ορίζει τον συγκριτή για την ταξινόμηση των εργασιών στο γράφημα Gantt και στο γράφημα Φύλλου Εργασιών."
type: docs
weight: 180
url: /el/net/aspose.tasks.saving/saveoptions/taskscomparer/
---
## SaveOptions.TasksComparer property

Λαμβάνει ή ορίζει τον συγκριτή για την ταξινόμηση των εργασιών στο γράφημα Gantt και στο γράφημα Φύλλου Εργασιών.

```csharp
public IComparer<Task> TasksComparer { get; set; }
```

### Παραδείγματα

Δείχνει πώς να ορίσετε έναν συγκριτή για την ταξινόμηση των εργασιών στο διάγραμμα Gantt και/ή στο διάγραμμα Φύλλου Εργασιών.

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

### Δείτε επίσης

* class [Task](../../../aspose.tasks/task)
* class [SaveOptions](../../saveoptions)
* namespace [Aspose.Tasks.Saving](../../saveoptions)
* assembly [Aspose.Tasks](../../../)

<!-- ΜΗ ΕΠΕΞΕΡΓΑΣΙΑ: δημιουργήθηκε από xmldocmd για Aspose.Tasks.dll -->
