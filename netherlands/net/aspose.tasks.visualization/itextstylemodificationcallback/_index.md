---
title: "Interface ITextStyleModificationCallback"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Visualization.ITextStyleModificationCallback interface. Vertegenwoordigt een callback die wordt aangeroepen voordat TextStyle wordt toegepast op een tabelcel."
type: docs
weight: 3160
url: /nl/net/aspose.tasks.visualization/itextstylemodificationcallback/
---
## ITextStyleModificationCallback interface

Stelt een callback voor die wordt aangeroepen voordat TextStyle wordt toegepast op een tabelcel.

```csharp
public interface ITextStyleModificationCallback
```

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [BeforeTaskTextStyleApplied](../../aspose.tasks.visualization/itextstylemodificationcallback/beforetasktextstyleapplied/)(TaskTextStyleEventArgs) | De methode die moet worden aangeroepen vóór het renderen van een tabelcel voor een taakrij in de volgende weergaven: 'Gantt Chart', 'Task Sheet', 'Task Usage'. |

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


