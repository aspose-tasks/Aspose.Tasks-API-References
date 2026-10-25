---
title: "Class TaskTextStyleEventArgs"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Visualization.TaskTextStyleEventArgs class. Bu sınıf, tablo hücrelerinin içeriğinin işlenmesiyle ilgili veri kümesini temsil eder."
type: docs
weight: 3390
url: /tr/net/aspose.tasks.visualization/tasktextstyleeventargs/
---
## TaskTextStyleEventArgs class

Bu sınıf, tablo hücresinin içeriğinin işlenmesiyle ilgili veri kümesini temsil eder.

```csharp
public class TaskTextStyleEventArgs
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CellTextStyle](../../aspose.tasks.visualization/tasktextstyleeventargs/celltextstyle/) { get; set; } | Hücre içeriğini çizmeye kullanılacak TextStyle'ı alır veya ayarlar. Bu nesne, bir tablo hücresinin görünümünü özelleştirmek için kullanılabilir. |
| [Column](../../aspose.tasks.visualization/tasktextstyleeventargs/column/) { get; } | Şu anda işlenen hücrenin ait olduğu [`ViewColumn`](../viewcolumn/) alır. |
| [Task](../../aspose.tasks.visualization/tasktextstyleeventargs/task/) { get; } | Şu anda işlenen satıra karşılık gelen [`Task`](./task/) alır. |

## Örnekler

Dışa aktarılacak görünüm sütunlarının nasıl ekleneceğini gösterir.

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

    // sütunlar üzerinde yinele
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
    /// Aşağıdaki görünümlerde görev satırı için bir tablo hücresinin işlenmesinden önce çağrılacak yöntem:
    /// 'Gantt Chart', 'Task Sheet', 'Task Usage'.
    /// </summary>
    /// <param name="args">Bu <see cref="T:Aspose.Tasks.Visualization.TaskTextStyleEventArgs" /> nesnesi.</param>
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

### Ayrıca Bakınız

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


