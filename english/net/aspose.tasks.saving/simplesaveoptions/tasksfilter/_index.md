---
title: SimpleSaveOptions.TasksFilter
second_title: Aspose.Tasks for .NET API Reference
description: SimpleSaveOptions property. Gets or sets the condition which is used to filter tasks rendered on Gantt Task Sheet and Task Usage charts
type: docs
weight: 30
url: /net/aspose.tasks.saving/simplesaveoptions/tasksfilter/
---
## SimpleSaveOptions.TasksFilter property

Gets or sets the condition which is used to filter tasks rendered on Gantt, Task Sheet and Task Usage charts.

```csharp
public ICondition<Task> TasksFilter { get; set; }
```

## Remarks

If value is not specified the default filter is used which removes non-visible tasks -- i.e. descendant tasks of collapsed tasks.

## Examples

Shows how to use custom tasks filter while saving MS Project file.

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

        // set a task filter to skip task 'Task5' and 'Task3'
        TasksFilter = new CustomTasksFilter()
    };

    // lets check the save format
    Console.WriteLine("The save format: " + options.SaveFormat);

    // ...

    // save the project as an image
    project.Save(OutDir + "WorkWithTasksFilter_out.png", options);
}

/// <summary>
/// Example of custom task filter that can be used while saving MS Project file (for instance) in PDF format.
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

### See Also

* interface [ICondition&lt;T&gt;](../../../aspose.tasks.util/icondition-1/)
* class [Task](../../../aspose.tasks/task/)
* class [SimpleSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../simplesaveoptions/)
* assembly [Aspose.Tasks](../../../)


