---
title: "AssignmentViewColumn.AssignmentViewColumn"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ AssignmentViewColumn. يهيئ نسخة جديدة من فئة AssignmentViewColumn"
type: docs
weight: 10
url: /ar/net/aspose.tasks.visualization/assignmentviewcolumn/assignmentviewcolumn/
---
## AssignmentViewColumn constructor

يُهيئ نسخة جديدة من فئة AssignmentViewColumn.

```csharp
public AssignmentViewColumn(string name, int width, AssignmentToColumnTextConverter converter)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| الاسم | سلسلة | اسم العمود. |
| العرض | Int32 | عرض العمود بالبكسل. |
| محول | AssignmentToColumnTextConverter | محول بيانات التعيين إلى نص العمود. |

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

* delegate [AssignmentToColumnTextConverter](../../assignmenttocolumntextconverter/)
* class [AssignmentViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../assignmentviewcolumn/)
* assembly [Aspose.Tasks](../../../)


