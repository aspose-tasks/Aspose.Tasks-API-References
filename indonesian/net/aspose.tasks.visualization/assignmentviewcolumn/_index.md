---
title: "Kelas AssignmentViewColumn"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Visualization.AssignmentViewColumn. Kelas tampilan proyek"
type: docs
weight: 2930
url: /id/net/aspose.tasks.visualization/assignmentviewcolumn/
---
## AssignmentViewColumn class

Kelas tampilan proyek.

```csharp
public class AssignmentViewColumn : ViewColumn
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [AssignmentViewColumn](assignmentviewcolumn/)(string, int, AssignmentToColumnTextConverter) | Menginisialisasi instance baru dari kelas AssignmentViewColumn. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| override [Field](../../aspose.tasks.visualization/assignmentviewcolumn/field/) { get; set; } | Kolom bidang. [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | Mendapatkan nama kolom. |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | Mendapatkan atau mengatur perataan teks (bisa menjadi salah satu nilai dari enumerasi [`HorizontalStringAlignment`](../horizontalstringalignment/)). |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | Mendapatkan atau mengatur callback yang dapat digunakan untuk menyesuaikan tampilan sel kolom. |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | Mendapatkan lebar kolom. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [GetColumnText](../../aspose.tasks.visualization/assignmentviewcolumn/getcolumntext/)(ResourceAssignment) | Mengonversi penugasan sumber daya saat ini menjadi teks kolom. |

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

* class [ViewColumn](../viewcolumn/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


