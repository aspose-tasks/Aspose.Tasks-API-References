---
title: "فئة TaskTextStyleEventArgs"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.Visualization.TaskTextStyleEventArgs. تمثل هذه الفئة مجموعة من البيانات المتعلقة برسم محتوى خلايا الجدول."
type: docs
weight: 3390
url: /ar/net/aspose.tasks.visualization/tasktextstyleeventargs/
---
## TaskTextStyleEventArgs class

هذه الفئة تمثل مجموعة من البيانات المتعلقة بعرض محتوى خلية الجدول.

```csharp
public class TaskTextStyleEventArgs
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CellTextStyle](../../aspose.tasks.visualization/tasktextstyleeventargs/celltextstyle/) { get; set; } | يحصل أو يعيّن TextStyle الذي سيُستخدم لرسم محتوى الخلية. يمكن استخدام هذا الكائن لتخصيص مظهر خلية الجدول. |
| [Column](../../aspose.tasks.visualization/tasktextstyleeventargs/column/) { get; } | يحصل على [`ViewColumn`](../viewcolumn/) التي تنتمي إليها الخلية المرسومة حاليًا. |
| [Task](../../aspose.tasks.visualization/tasktextstyleeventargs/task/) { get; } | يحصل على [`Task`](./task/) التي تتطابق مع الصف المرسوم حاليًا. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


