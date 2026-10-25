---
title: "SimpleSaveOptions.TasksComparer"
second_title: "Aspose.Tasks for .NET API 참조"
description: "SimpleSaveOptions 속성. Gantt 차트와 작업 시트 차트에서 작업을 정렬하기 위한 비교자를 가져오거나 설정합니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks.saving/simplesaveoptions/taskscomparer/
---
## SimpleSaveOptions.TasksComparer property

간트 차트 및 작업 시트 차트에서 작업을 정렬하기 위한 비교자를 가져오거나 설정합니다.

```csharp
public IComparer<Task> TasksComparer { get; set; }
```

## 예제

Gantt 차트 및/또는 작업 시트 차트에서 작업을 정렬하기 위한 비교자를 설정하는 방법을 보여줍니다.

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

### 또 보기

* class [Task](../../../aspose.tasks/task/)
* class [SimpleSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../simplesaveoptions/)
* assembly [Aspose.Tasks](../../../)


