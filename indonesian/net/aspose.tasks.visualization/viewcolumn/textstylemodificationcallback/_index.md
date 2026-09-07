---
title: "ViewColumn.TextStyleModificationCallback"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti ViewColumn. Mendapatkan atau mengatur callback yang dapat digunakan untuk menyesuaikan tampilan sel kolom."
type: docs
weight: 40
url: /id/net/aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/
---
## ViewColumn.TextStyleModificationCallback property

Mendapatkan atau mengatur callback yang dapat digunakan untuk menyesuaikan tampilan sel kolom.

```csharp
public ITextStyleModificationCallback TextStyleModificationCallback { get; set; }
```

## Contoh

Menampilkan cara menambahkan kolom tampilan yang akan diekspor.

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

    // iterasi melalui kolom
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
    /// Metode yang akan dipanggil sebelum merender sel tabel untuk baris tugas dalam tampilan berikut:
    /// 'Gantt Chart', 'Task Sheet', 'Task Usage'.
    /// </summary>
    /// <param name="args">Objek <see cref="T:Aspose.Tasks.Visualization.TaskTextStyleEventArgs" />.</param>
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

### Lihat Juga

* interface [ITextStyleModificationCallback](../../itextstylemodificationcallback/)
* class [ViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../viewcolumn/)
* assembly [Aspose.Tasks](../../../)


