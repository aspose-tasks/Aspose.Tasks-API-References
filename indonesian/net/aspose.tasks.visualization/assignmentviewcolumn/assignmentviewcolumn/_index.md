---
title: "AssignmentViewColumn.AssignmentViewColumn"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor AssignmentViewColumn. Menginisialisasi instance baru dari kelas AssignmentViewColumn."
type: docs
weight: 10
url: /id/net/aspose.tasks.visualization/assignmentviewcolumn/assignmentviewcolumn/
---
## AssignmentViewColumn constructor

Menginisialisasi instance baru dari kelas AssignmentViewColumn.

```csharp
public AssignmentViewColumn(string name, int width, AssignmentToColumnTextConverter converter)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nama | String | Nama kolom. |
| lebar | Int32 | Lebar kolom dalam piksel. |
| konverter | AssignmentToColumnTextConverter | Konverter data penugasan ke teks kolom. |

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

* delegate [AssignmentToColumnTextConverter](../../assignmenttocolumntextconverter/)
* class [AssignmentViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../assignmentviewcolumn/)
* assembly [Aspose.Tasks](../../../)


