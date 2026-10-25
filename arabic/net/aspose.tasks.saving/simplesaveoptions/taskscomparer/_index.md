---
title: "SimpleSaveOptions.TasksComparer"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية SimpleSaveOptions. تحصل أو تعيين المقارن لترتيب المهام على مخطط جانت ومخطط ورقة المهام"
type: docs
weight: 20
url: /ar/net/aspose.tasks.saving/simplesaveoptions/taskscomparer/
---
## SimpleSaveOptions.TasksComparer property

يحصل أو يعيّن المقارن لفرز المهام على مخطط جانت ومخطط ورقة المهام.

```csharp
public IComparer<Task> TasksComparer { get; set; }
```

## الأمثلة

يوضح كيفية تعيين مقارن لفرز المهام على مخطط جانت و/أو مخطط ورقة المهام.

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

### انظر أيضًا

* class [Task](../../../aspose.tasks/task/)
* class [SimpleSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../simplesaveoptions/)
* assembly [Aspose.Tasks](../../../)


