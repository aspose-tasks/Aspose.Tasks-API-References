---
title: "ViewColumn.TextStyleModificationCallback"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ViewColumn özelliği. Sütun hücrelerinin görünümünü özelleştirmek için kullanılabilecek geri çağırmayı alır veya ayarlar."
type: docs
weight: 40
url: /tr/net/aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/
---
## ViewColumn.TextStyleModificationCallback property

Sütun hücrelerinin görünümünü özelleştirmek için kullanılabilecek geri çağırmayı alır veya ayarlar.

```csharp
public ITextStyleModificationCallback TextStyleModificationCallback { get; set; }
```

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

* interface [ITextStyleModificationCallback](../../itextstylemodificationcallback/)
* class [ViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../viewcolumn/)
* assembly [Aspose.Tasks](../../../)


