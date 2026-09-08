---
title: "Aspose.Tasks.Visualization.ViewColumn class. Vertegenwoordigt een kolom in een projectweergave."
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Haalt het kolomveld op of stelt het in. [`Field`](./field/)."
type: docs
weight: 3470
url: /nl/net/aspose.tasks.visualization/viewcolumn/
---
## ViewColumn class

Stelt een kolom in een projectweergave voor.

```csharp
public abstract class ViewColumn
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| abstract [Field](../../aspose.tasks.visualization/viewcolumn/field/) { get; set; } | Class Gridlines |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | Haalt de kolomnaam op. |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | Haalt de uitlijning van de tekst op of stelt deze in (kan een van de waarden van de enumeratie [`HorizontalStringAlignment`](../horizontalstringalignment/) zijn). |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | Haalt de callback op of stelt deze in die kan worden gebruikt om het uiterlijk van de cellen van de kolom aan te passen. |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | Haalt de kolombreedte op. |

## Voorbeelden

Toont hoe weergavekolommen toe te voegen die geëxporteerd moeten worden.

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

    // itereren over kolommen
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
    /// De methode die moet worden aangeroepen vóór het renderen van een tabelcel voor een taakrij in de volgende weergaven:
    /// 'Gantt Chart', 'Task Sheet', 'Task Usage'.
    /// </summary>
    /// <param name=\"args\">Het <see cref=\"T:Aspose.Tasks.Visualization.TaskTextStyleEventArgs\" /> object.</param>
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

### Zie ook

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


