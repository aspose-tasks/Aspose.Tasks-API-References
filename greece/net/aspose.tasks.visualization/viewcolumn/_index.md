---
title: "Κλάση ViewColumn"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Visualization.ViewColumn class. Αντιπροσωπεύει μια στήλη σε προβολή έργου"
type: docs
weight: 3470
url: /el/net/aspose.tasks.visualization/viewcolumn/
---
## ViewColumn class

Αντιπροσωπεύει μια στήλη σε προβολή έργου.

```csharp
public abstract class ViewColumn
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| abstract [Field](../../aspose.tasks.visualization/viewcolumn/field/) { get; set; } | Λαμβάνει ή ορίζει το πεδίο στήλης. [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | Λαμβάνει το όνομα της στήλης. |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | Λαμβάνει ή ορίζει την ευθυγράμμιση του κειμένου (μπορεί να είναι μία από τις τιμές της απαρίθμησης [`HorizontalStringAlignment`](../horizontalstringalignment/)). |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | Λαμβάνει ή ορίζει την κλήση επιστροφής (callback) που μπορεί να χρησιμοποιηθεί για την προσαρμογή της εμφάνισης των κελιών της στήλης. |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | Λαμβάνει το πλάτος της στήλης. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


