---
title: SimpleSaveOptions.SaveFormat
second_title: Aspose.Tasks for .NET API Reference
description: SimpleSaveOptions property. Gets or sets the format in which the document will be saved if this save options object is used
type: docs
weight: 10
url: /net/aspose.tasks.saving/simplesaveoptions/saveformat/
---
## SimpleSaveOptions.SaveFormat property

Gets or sets the format in which the document will be saved if this save options object is used.

```csharp
public SaveFileFormat SaveFormat { get; }
```

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

* enum [SaveFileFormat](../../savefileformat/)
* class [SimpleSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../simplesaveoptions/)
* assembly [Aspose.Tasks](../../../)


