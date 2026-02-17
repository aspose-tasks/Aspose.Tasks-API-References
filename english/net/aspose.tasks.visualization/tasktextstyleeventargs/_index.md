---
title: Class TaskTextStyleEventArgs
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.TaskTextStyleEventArgs class. This class represents set of data that related to the rendering of table cells content
type: docs
weight: 3370
url: /net/aspose.tasks.visualization/tasktextstyleeventargs/
---
## TaskTextStyleEventArgs class

This class represents set of data that related to the rendering of table cell's content.

```csharp
public class TaskTextStyleEventArgs
```

## Properties

| Name | Description |
| --- | --- |
| [CellTextStyle](../../aspose.tasks.visualization/tasktextstyleeventargs/celltextstyle/) { get; set; } | Gets or sets TextStyle which will be used to draw the cell's content. This object can be use to customize appearance of a table cell. |
| [Column](../../aspose.tasks.visualization/tasktextstyleeventargs/column/) { get; } | Gets [`ViewColumn`](../viewcolumn/) to which the currently rendered cell belongs. |
| [Task](../../aspose.tasks.visualization/tasktextstyleeventargs/task/) { get; } | Gets [`Task`](./task/) which corresponds to the currently rendered row. |

## Examples

Shows how to add view columns to be exported.

```csharp
public void WorkWithViewColumn()
{
    var project = new Project(DataDir + "Project2.mpp");

    var options = new PdfSaveOptions();
    var columns = new List<ViewColumn>
    {
        new ResourceViewColumn(100, Field.ResourceName),
        new ResourceViewColumn(100, Field.ResourceActualWork),
        new ResourceViewColumn(100, Field.ResourceCost)
    };

    columns[0].TextStyleModificationCallback = new MyTextStyleCallback();

    // iterate over columns
    foreach (var column in columns)
    {
        Console.WriteLine("Column Name: " + column.Name);
        Console.WriteLine("Column Field: " + column.Field);
        Console.WriteLine("Column Width: " + column.Width);
        Console.WriteLine("Column Callback: " + column.TextStyleModificationCallback);
        Console.WriteLine();
    }

    options.View = new ProjectView(columns);
    options.PresentationFormat = PresentationFormat.ResourceUsage;

    project.Save(OutDir + "WorkWithViewColumn_out.pdf", options);
}

private class MyTextStyleCallback : ITextStyleModificationCallback
{
    /// <summary>
    /// The method to be called before rendering of a table cell for a task row in the following views:
    /// 'Gantt Chart', 'Task Sheet', 'Task Usage'.
    /// </summary>
    /// <param name="args">The <see cref="T:Aspose.Tasks.Visualization.TaskTextStyleEventArgs" /> object.</param>
    public void BeforeTaskTextStyleApplied(TaskTextStyleEventArgs args)
    {
        if (args.Task.Get(Tsk.Uid) % 2 == 0)
        {
            args.CellTextStyle.BackgroundColor = 
                args.Column.StringAlignment == HorizontalStringAlignment.Center 
                ? Color.Cyan : Color.Red;
            args.CellTextStyle.BackgroundPattern = BackgroundPattern.SolidFill;
        }
        else
        {
            args.CellTextStyle.Color = Color.DarkGreen;
        }
    }
}
```

### See Also

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


