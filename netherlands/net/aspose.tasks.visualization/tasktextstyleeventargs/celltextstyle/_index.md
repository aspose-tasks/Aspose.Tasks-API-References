---
title: "TaskTextStyleEventArgs.CellTextStyle"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TaskTextStyleEventArgs eigenschap. Haalt of stelt TextStyle in dat zal worden gebruikt om de inhoud van de cellen te tekenen. Dit object kan worden gebruikt om het uiterlijk van een tabelcel aan te passen."
type: docs
weight: 10
url: /nl/net/aspose.tasks.visualization/tasktextstyleeventargs/celltextstyle/
---
## TaskTextStyleEventArgs.CellTextStyle property

Haalt [`ViewColumn`](../viewcolumn/) op waartoe de momenteel gerenderde cel behoort.

```csharp
public TextStyle CellTextStyle { get; set; }
```

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

* class [TextStyle](../../textstyle/)
* class [TaskTextStyleEventArgs](../)
* namespace [Aspose.Tasks.Visualization](../../tasktextstyleeventargs/)
* assembly [Aspose.Tasks](../../../)


