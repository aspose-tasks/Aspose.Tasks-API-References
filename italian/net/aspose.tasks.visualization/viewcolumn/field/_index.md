---
title: "ViewColumn.Field"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà ViewColumn. Ottiene o imposta il campo della colonna. Field"
type: docs
weight: 10
url: /it/net/aspose.tasks.visualization/viewcolumn/field/
---
## ViewColumn.Field property

Ottiene o imposta il campo della colonna. `Field`.

```csharp
public abstract Field Field { get; set; }
```

## Esempi

Mostra come aggiungere colonne di visualizzazione da esportare.

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

    // itera sulle colonne
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
    /// Il metodo da chiamare prima del rendering di una cella di tabella per una riga di attività nelle seguenti visualizzazioni:
    /// 'Gantt Chart', 'Task Sheet', 'Task Usage'.
    /// </summary>
    /// <param name="args">L'oggetto <see cref="T:Aspose.Tasks.Visualization.TaskTextStyleEventArgs" />.</param>
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

### Vedi anche

* enum [Field](../../../aspose.tasks/field/)
* class [ViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../viewcolumn/)
* assembly [Aspose.Tasks](../../../)


