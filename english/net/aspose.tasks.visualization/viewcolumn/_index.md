---
title: Class ViewColumn
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Visualization.ViewColumn class. Represents a column in a project view
type: docs
weight: 3440
url: /net/aspose.tasks.visualization/viewcolumn/
---
## ViewColumn class

Represents a column in a project view.

```csharp
public abstract class ViewColumn
```

## Properties

| Name | Description |
| --- | --- |
| abstract [Field](../../aspose.tasks.visualization/viewcolumn/field/) { get; set; } | Gets or sets column field. [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | Gets the column name. |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | Gets or sets alignment of the text (can be one of the values of the [`HorizontalStringAlignment`](../horizontalstringalignment/) enumeration). |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | Gets or sets the callback which can be used to customize the appearance of the column's cells. |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | Gets the column width. |

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


