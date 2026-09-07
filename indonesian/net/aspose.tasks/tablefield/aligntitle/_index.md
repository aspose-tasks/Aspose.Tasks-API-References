---
title: "TableField.AlignTitle"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti TableField. Mendapatkan atau mengatur perataan judul dalam bidang tabel"
type: docs
weight: 30
url: /id/net/aspose.tasks/tablefield/aligntitle/
---
## TableField.AlignTitle property

Mendapatkan atau mengatur perataan judul dalam bidang tabel.

```csharp
public HorizontalStringAlignment AlignTitle { get; set; }
```

## Contoh

Menampilkan cara membaca tabel proyek.

```csharp
var project = new Project(DataDir + "ReadTableData.mpp");

// dapatkan tabel
var table = project.Tables.ToList()[0];
Console.WriteLine("Print table fields of {0}", table.Name);
Console.WriteLine("Table Fields Count" + table.TableFields.Count);

// tampilkan semua informasi bidang tabel
foreach (var field in table.TableFields)
{
    Console.WriteLine("  Field: " + field.Field);
    Console.WriteLine("  Width: " + field.Width);
    Console.WriteLine("  Title: " + field.Title);
    Console.WriteLine("  Title Alignment: " + field.AlignTitle);
    Console.WriteLine("  Data Alignment: " + field.AlignData);
    Console.WriteLine("  Wrap Header: " + field.WrapHeader);
    Console.WriteLine("  Wrap Text: " + field.WrapText);
    Console.WriteLine();
}
```

### Lihat Juga

* enum [HorizontalStringAlignment](../../../aspose.tasks.visualization/horizontalstringalignment/)
* class [TableField](../)
* namespace [Aspose.Tasks](../../tablefield/)
* assembly [Aspose.Tasks](../../../)


