---
title: "TaskTextStyleEventArgs.CellTextStyle"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية TaskTextStyleEventArgs. تحصل أو تعين TextStyle التي ستُستخدم لرسم محتوى الخلايا. يمكن استخدام هذا الكائن لتخصيص مظهر خلية الجدول."
type: docs
weight: 10
url: /ar/net/aspose.tasks.visualization/tasktextstyleeventargs/celltextstyle/
---
## TaskTextStyleEventArgs.CellTextStyle property

يحصل أو يعيّن TextStyle الذي سيُستخدم لرسم محتوى الخلية. يمكن استخدام هذا الكائن لتخصيص مظهر خلية الجدول.

```csharp
public TextStyle CellTextStyle { get; set; }
```

## الأمثلة

يوضح كيفية إضافة أعمدة العرض للتصدير.

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

    // التكرار عبر الأعمدة
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
    /// الطريقة التي سيتم استدعاؤها قبل رسم خلية جدول لصف مهمة في العروض التالية:
    /// 'Gantt Chart'، 'Task Sheet'، 'Task Usage'.
    /// </summary>
    /// <param name="args">الكائن <see cref="T:Aspose.Tasks.Visualization.TaskTextStyleEventArgs" />.</param>
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

### انظر أيضًا

* class [TextStyle](../../textstyle/)
* class [TaskTextStyleEventArgs](../)
* namespace [Aspose.Tasks.Visualization](../../tasktextstyleeventargs/)
* assembly [Aspose.Tasks](../../../)


