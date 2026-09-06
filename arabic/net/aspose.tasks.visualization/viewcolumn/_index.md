---
title: "فئة ViewColumn"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.Visualization.ViewColumn. تمثل عمودًا في عرض المشروع."
type: docs
weight: 3470
url: /ar/net/aspose.tasks.visualization/viewcolumn/
---
## ViewColumn class

يمثل عمودًا في عرض المشروع.

```csharp
public abstract class ViewColumn
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| abstract [Field](../../aspose.tasks.visualization/viewcolumn/field/) { get; set; } | يحصل أو يعيّن حقل العمود. [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | يحصل على اسم العمود. |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | يحصل أو يعيّن محاذاة النص (يمكن أن تكون أحد قيم تعداد [`HorizontalStringAlignment`](../horizontalstringalignment/)). |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | يحصل أو يعيّن رد النداء الذي يمكن استخدامه لتخصيص مظهر خلايا العمود. |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | يحصل على عرض العمود. |

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


