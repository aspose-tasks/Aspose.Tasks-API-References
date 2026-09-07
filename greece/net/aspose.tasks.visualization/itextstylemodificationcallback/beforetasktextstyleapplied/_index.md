---
title: "ITextStyleModificationCallback.BeforeTaskTextStyleApplied"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος ITextStyleModificationCallback. Η μέθοδος που καλείται πριν από την απόδοση ενός κελιού πίνακα για μια γραμμή εργασίας στις ακόλουθες προβολές Gantt Chart Task Sheet Task Usage"
type: docs
weight: 10
url: /el/net/aspose.tasks.visualization/itextstylemodificationcallback/beforetasktextstyleapplied/
---
## ITextStyleModificationCallback.BeforeTaskTextStyleApplied method

Η μέθοδος που θα κληθεί πριν από την απόδοση ενός κελιού πίνακα για μια σειρά εργασίας στις ακόλουθες προβολές: 'Gantt Chart', 'Task Sheet', 'Task Usage'.

```csharp
public void BeforeTaskTextStyleApplied(TaskTextStyleEventArgs args)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| args | TaskTextStyleEventArgs | Το αντικείμενο [`TaskTextStyleEventArgs`](../../tasktextstyleeventargs/). |

## Παραδείγματα

Δείχνει πώς να προσθέσετε στήλες προβολής για εξαγωγή.

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

    // επανάληψη στις στήλες
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
    /// Η μέθοδος που θα κληθεί πριν από την απόδοση ενός κελιού πίνακα για μια σειρά εργασίας στις ακόλουθες προβολές:
    /// 'Gantt Chart', 'Task Sheet', 'Task Usage'.
    /// </summary>
    /// <param name="args">Το <see cref="T:Aspose.Tasks.Visualization.TaskTextStyleEventArgs" /> object.</param>
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

### Δείτε επίσης

* class [TaskTextStyleEventArgs](../../tasktextstyleeventargs/)
* interface [ITextStyleModificationCallback](../)
* namespace [Aspose.Tasks.Visualization](../../itextstylemodificationcallback/)
* assembly [Aspose.Tasks](../../../)


