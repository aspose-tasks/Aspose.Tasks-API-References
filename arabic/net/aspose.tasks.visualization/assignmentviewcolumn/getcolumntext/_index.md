---
title: "AssignmentViewColumn.GetColumnText"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة AssignmentViewColumn. تحول تعيين المورد الحالي إلى نص العمود"
type: docs
weight: 30
url: /ar/net/aspose.tasks.visualization/assignmentviewcolumn/getcolumntext/
---
## AssignmentViewColumn.GetColumnText method

يحوّل تعيين المورد الحالي إلى نص العمود.

```csharp
public string GetColumnText(ResourceAssignment assignment)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| تعيين | ResourceAssignment | التعيين الحالي. |

### قيمة الإرجاع

نص العمود.

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

* class [ResourceAssignment](../../../aspose.tasks/resourceassignment/)
* class [AssignmentViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../assignmentviewcolumn/)
* assembly [Aspose.Tasks](../../../)


