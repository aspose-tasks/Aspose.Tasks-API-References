---
title: "Class TaskTextStyleEventArgs"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.Visualization.TaskTextStyleEventArgs classe. Questa classe rappresenta un insieme di dati relativi al rendering del contenuto delle celle di tabella."
type: docs
weight: 3390
url: /it/net/aspose.tasks.visualization/tasktextstyleeventargs/
---
## TaskTextStyleEventArgs class

Questa classe rappresenta un insieme di dati correlati al rendering del contenuto delle celle della tabella.

```csharp
public class TaskTextStyleEventArgs
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CellTextStyle](../../aspose.tasks.visualization/tasktextstyleeventargs/celltextstyle/) { get; set; } | Ottiene o imposta TextStyle che verrà usato per disegnare il contenuto della cella. Questo oggetto può essere usato per personalizzare l'aspetto di una cella di tabella. |
| [Column](../../aspose.tasks.visualization/tasktextstyleeventargs/column/) { get; } | Ottiene [`ViewColumn`](../viewcolumn/) a cui appartiene la cella attualmente renderizzata. |
| [Task](../../aspose.tasks.visualization/tasktextstyleeventargs/task/) { get; } | Ottiene [`Task`](./task/) che corrisponde alla riga attualmente renderizzata. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


