---
title: "الفئة AssignmentViewColumn"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.Visualization.AssignmentViewColumn. فئة عرض المشاريع"
type: docs
weight: 2930
url: /ar/net/aspose.tasks.visualization/assignmentviewcolumn/
---
## AssignmentViewColumn class

فئة عرض المشروع.

```csharp
public class AssignmentViewColumn : ViewColumn
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [AssignmentViewColumn](assignmentviewcolumn/)(string, int, AssignmentToColumnTextConverter) | يُهيئ نسخة جديدة من فئة AssignmentViewColumn. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| override [Field](../../aspose.tasks.visualization/assignmentviewcolumn/field/) { get; set; } | حقل العمود. [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | يحصل على اسم العمود. |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | يحصل أو يعيّن محاذاة النص (يمكن أن تكون أحد قيم تعداد [`HorizontalStringAlignment`](../horizontalstringalignment/)). |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | يحصل أو يعيّن رد النداء الذي يمكن استخدامه لتخصيص مظهر خلايا العمود. |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | يحصل على عرض العمود. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [GetColumnText](../../aspose.tasks.visualization/assignmentviewcolumn/getcolumntext/)(ResourceAssignment) | يحوّل تعيين المورد الحالي إلى نص العمود. |

## الأمثلة

يعرض كيفية إضافة أعمدة لعرض التعيينات.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new Spreadsheet2003SaveOptions();

var column = new AssignmentViewColumn("Notes", 200, delegate(ResourceAssignment assignment) { return assignment.Get(Asn.NotesText); });
options.AssignmentView.Columns.Add(column);

foreach (var assignment in project.ResourceAssignments)
{
    foreach (var col in options.AssignmentView.Columns)
    {
        var assnCol = (AssignmentViewColumn)col;
        Console.WriteLine("Column Field: " + assnCol.Field);
        Console.WriteLine("Column Text ( converted ): " + assnCol.GetColumnText(assignment));
        Console.WriteLine();
    }
}

project.Save(OutDir + "UsingSpreadsheet2003SaveOptions_out.xml", options);
```

### انظر أيضًا

* class [ViewColumn](../viewcolumn/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


