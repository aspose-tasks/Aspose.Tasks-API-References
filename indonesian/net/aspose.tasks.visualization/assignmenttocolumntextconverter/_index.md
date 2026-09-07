---
title: "Delegasi AssignmentToColumnTextConverter"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konverter string data ResourceAssignment ke kolom"
type: docs
weight: 2920
url: /id/net/aspose.tasks.visualization/assignmenttocolumntextconverter/
---
## AssignmentToColumnTextConverter delegate

Konverter data ResourceAssignment ke string kolom.

```csharp
public delegate string AssignmentToColumnTextConverter(ResourceAssignment assignment);
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| penugasan | ResourceAssignment | Penugasan yang akan dikonversi. |

### Nilai Kembali

Data string untuk kolom.

## Contoh

Menampilkan cara menambahkan kolom untuk tampilan penugasan.

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

### Lihat Juga

* class [ResourceAssignment](../../aspose.tasks/resourceassignment/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


