---
title: "SimpleSaveOptions.TasksFilter"
second_title: "Aspose.Tasks for .NET API 参考"
description: "SimpleSaveOptions 属性。获取或设置用于过滤在甘特任务表和任务使用图表上呈现的任务的条件"
type: docs
weight: 30
url: /zh/net/aspose.tasks.saving/simplesaveoptions/tasksfilter/
---
## SimpleSaveOptions.TasksFilter property

获取或设置用于过滤在甘特图、任务表和任务使用图上渲染的任务的条件。

```csharp
public ICondition<Task> TasksFilter { get; set; }
```

## 备注

如果未指定值，将使用默认过滤器，该过滤器会移除不可见的任务——即折叠任务的子任务。

## 示例

展示如何在保存 MS Project 文件时使用自定义任务过滤器。

```csharp
public void WorkWithTasksFilter()
{
    var project = new Project(DataDir + "CreateProject2.mpp");

    var options = new PdfSaveOptions
    {
        PresentationFormat = PresentationFormat.GanttChart,
        PageSize = PageSize.A3,
        StartDate = new DateTime(2010, 7, 1),
        EndDate = new DateTime(2010, 9, 1),

        // 设置任务过滤器以跳过任务 'Task5' 和 'Task3'
        TasksFilter = new CustomTasksFilter()
    };

    // 让我们检查保存格式
    Console.WriteLine("The save format: " + options.SaveFormat);

    // ...

    // 将项目保存为图像
    project.Save(OutDir + "WorkWithTasksFilter_out.png", options);
}

/// <summary>
/// 示例可在保存 MS Project 文件（例如）为 PDF 格式时使用的自定义任务过滤器。
/// </summary>
/// <inheritdoc />
private class CustomTasksFilter : ICondition<Task>
{
    public bool Check(Task el)
    {
        return el.Get(Tsk.Name) != "Task5" && el.Get(Tsk.Name) != "Task3";
    }
}
```

### 另见

* interface [ICondition&lt;T&gt;](../../../aspose.tasks.util/icondition-1/)
* class [Task](../../../aspose.tasks/task/)
* class [SimpleSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../simplesaveoptions/)
* assembly [Aspose.Tasks](../../../)


