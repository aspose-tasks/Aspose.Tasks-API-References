---
title: "ResourceViewColumn.GetColumnText"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode ResourceViewColumn. Mengonversi sumber daya saat ini ke teks kolom"
type: docs
weight: 30
url: /id/net/aspose.tasks.visualization/resourceviewcolumn/getcolumntext/
---
## ResourceViewColumn.GetColumnText method

Mengonversi sumber daya saat ini menjadi teks kolom.

```csharp
public string GetColumnText(Resource resource)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sumber daya | Sumber Daya | Sumber daya saat ini. |

### Nilai Kembali

Teks kolom.

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

* class [Resource](../../../aspose.tasks/resource/)
* class [ResourceViewColumn](../)
* namespace [Aspose.Tasks.Visualization](../../resourceviewcolumn/)
* assembly [Aspose.Tasks](../../../)


