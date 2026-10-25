---
title: "Kelas TableField"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.TableField. Mewakili bidang tabel dalam sebuah proyek"
type: docs
weight: 2340
url: /id/net/aspose.tasks/tablefield/
---
## TableField class

Mewakili sebuah bidang tabel dalam proyek.

```csharp
public class TableField
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [TableField](tablefield/)() | Menginisialisasi instance baru dari kelas `TableField`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [AlignData](../../aspose.tasks/tablefield/aligndata/) { get; set; } | Mendapatkan atau mengatur perataan data dalam bidang tabel. |
| [AlignTitle](../../aspose.tasks/tablefield/aligntitle/) { get; set; } | Mendapatkan atau mengatur perataan judul dalam bidang tabel. |
| [Field](../../aspose.tasks/tablefield/field/) { get; set; } | Mendapatkan atau mengatur tipe bidang tabel. |
| [Title](../../aspose.tasks/tablefield/title/) { get; set; } | Mendapatkan atau mengatur judul bidang dalam tabel. |
| [Width](../../aspose.tasks/tablefield/width/) { get; set; } | Mendapatkan atau mengatur lebar dalam poin kolom bidang dalam tabel. |
| [WrapHeader](../../aspose.tasks/tablefield/wrapheader/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah judul kolom tabel dapat membungkus ke beberapa baris, atau harus dipotong ketika melebihi lebar kolom. |
| [WrapText](../../aspose.tasks/tablefield/wraptext/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah teks kolom dapat membungkus ke beberapa baris, atau harus dipotong ketika melebihi lebar kolom. Didukung oleh versi MSP 2010 dan yang lebih baru. |

## Contoh

Menampilkan cara bekerja dengan tampilan Project dan menambahkan kolom ke tampilan default (yang ditampilkan ketika file MPP dibuka di MS Project).

```csharp
// buat proyek kosong tanpa tampilan
var project = new Project();
project.Set(Prj.Name, "Test View Project");

// Modifikasi tampilan default (ini adalah tampilan diagram Gantt).
// Atau Anda dapat memilih tampilan berdasarkan nama atau melalui Layar Tampilan menggunakan koleksi project.View.
var view = (GanttChartView) project.DefaultView;

TableField newColumn = new TableField()
{
    AlignData = HorizontalStringAlignment.Center,
    Title = "My new column",
    Width = 30,
    Field = Field.TaskActualDuration
};

view.Table.TableFields.Add(newColumn);

// Flag WriteViewData harus digunakan untuk menyimpan perubahan properti tampilan.
project.Save(OutDir + "ModifyView_output.mpp", new Saving.MPPSaveOptions
{
    WriteViewData = true
});
```

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


