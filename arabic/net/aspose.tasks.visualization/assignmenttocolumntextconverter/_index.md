---
title: "المندوب AssignmentToColumnTextConverter"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "محول بيانات ResourceAssignment إلى سلسلة الأعمدة"
type: docs
weight: 2920
url: /ar/net/aspose.tasks.visualization/assignmenttocolumntextconverter/
---
## AssignmentToColumnTextConverter delegate

محول بيانات ResourceAssignment إلى سلسلة العمود.

```csharp
public delegate string AssignmentToColumnTextConverter(ResourceAssignment assignment);
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| تعيين | ResourceAssignment | التعيين المراد تحويله. |

### قيمة الإرجاع

بيانات السلسلة للعمود.

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

* class [ResourceAssignment](../../aspose.tasks/resourceassignment/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


