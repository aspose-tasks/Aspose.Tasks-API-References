---
title: "Kelas ResourceViewColumn"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Visualization.ResourceViewColumn. Kelas tampilan proyek yang digunakan dalam tampilan ResourceUsage dan tampilan ResourceSheet"
type: docs
weight: 3350
url: /id/net/aspose.tasks.visualization/resourceviewcolumn/
---
## ResourceViewColumn class

Kelas tampilan proyek yang digunakan dalam tampilan ResourceUsage dan tampilan ResourceSheet.

```csharp
public sealed class ResourceViewColumn : ViewColumn
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [ResourceViewColumn](resourceviewcolumn/#constructor)(int, Field) | Menginisialisasi instance baru dari kelas `ResourceViewColumn`. |
| [ResourceViewColumn](resourceviewcolumn/#constructor_1)(string, int, ResourceToColumnTextConverter) | Menginisialisasi instance baru dari kelas `ResourceViewColumn`. |
| [ResourceViewColumn](resourceviewcolumn/#constructor_2)(string, int, ResourceToColumnTextConverter, Field) | Menginisialisasi instance baru dari kelas `ResourceViewColumn`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| override [Field](../../aspose.tasks.visualization/resourceviewcolumn/field/) { get; set; } | Kolom bidang. [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | Mendapatkan nama kolom. |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | Mendapatkan atau mengatur perataan teks (bisa menjadi salah satu nilai dari enumerasi [`HorizontalStringAlignment`](../horizontalstringalignment/)). |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | Mendapatkan atau mengatur callback yang dapat digunakan untuk menyesuaikan tampilan sel kolom. |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | Mendapatkan lebar kolom. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [GetColumnText](../../aspose.tasks.visualization/resourceviewcolumn/getcolumntext/)(Resource) | Mengonversi sumber daya saat ini menjadi teks kolom. |

## Contoh

Menampilkan cara menambahkan kolom tampilan sumber daya yang akan diekspor.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var resource = project.Resources.GetById(1);

var options = new PdfSaveOptions();
var columns = new List<ViewColumn>
{
    new ResourceViewColumn(100, Field.ResourceName),
    new ResourceViewColumn(100, Field.ResourceActualWork),
    new ResourceViewColumn(100, Field.ResourceCost),
    new ResourceViewColumn(
        "Resource Cost2", 
        80,
        delegate(Resource res)
        {
            return res.Get(Rsc.Cost).ToString(CultureInfo.InvariantCulture);
        }),
    new ResourceViewColumn(
        "Resource Cost2", 
        80,
        delegate(Resource res)
        {
            return res.Get(Rsc.Cost).ToString(CultureInfo.InvariantCulture);
        }, 
        Field.ResourceCost2)
};

// iterasi melalui kolom
foreach (var column in columns)
{
    var col = (ResourceViewColumn)column;
    Console.WriteLine("Column Name: " + col.Name);
    Console.WriteLine("Column Field: " + col.Field);
    Console.WriteLine("Column Text: " + col.GetColumnText(resource));
    Console.WriteLine();
}

options.View = new ProjectView(columns);
options.PresentationFormat = PresentationFormat.ResourceUsage;
project.Save(OutDir + "WorkWithAssignmentViewColumn_out.pdf", options);
```

### Lihat Juga

* class [ViewColumn](../viewcolumn/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


