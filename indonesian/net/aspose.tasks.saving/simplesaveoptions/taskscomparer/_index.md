---
title: "SimpleSaveOptions.TasksComparer"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti SimpleSaveOptions. Mendapatkan atau mengatur pembanding untuk mengurutkan tugas pada diagram Gantt dan diagram Lembar Tugas"
type: docs
weight: 20
url: /id/net/aspose.tasks.saving/simplesaveoptions/taskscomparer/
---
## SimpleSaveOptions.TasksComparer property

Mendapatkan atau mengatur pembanding untuk mengurutkan tugas pada diagram Gantt dan diagram Lembar Tugas.

```csharp
public IComparer<Task> TasksComparer { get; set; }
```

## Contoh

Menampilkan cara mengatur pembanding untuk mengurutkan tugas pada diagram Gantt dan/atau diagram Lembar Tugas.

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

### Lihat Juga

* class [Task](../../../aspose.tasks/task/)
* class [SimpleSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../simplesaveoptions/)
* assembly [Aspose.Tasks](../../../)


