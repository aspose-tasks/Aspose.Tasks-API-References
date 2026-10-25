---
title: "AssignmentViewColumn.GetColumnText"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode AssignmentViewColumn. Mengonversi penugasan sumber daya saat ini ke teks kolom"
type: docs
weight: 30
url: /id/net/aspose.tasks.visualization/assignmentviewcolumn/getcolumntext/
---
## AssignmentViewColumn.GetColumnText method

Mengonversi penugasan sumber daya saat ini menjadi teks kolom.

```csharp
public string GetColumnText(ResourceAssignment assignment)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| penugasan | ResourceAssignment | Penugasan saat ini. |

### Nilai Kembali

Teks kolom.

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

* class [ResourceAssignment](../../../aspose.tasks/resourceassignment/)
* class [AssignmentViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../assignmentviewcolumn/)
* assembly [Aspose.Tasks](../../../)


