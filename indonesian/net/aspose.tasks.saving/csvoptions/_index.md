---
title: "Kelas CsvOptions"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Saving.CsvOptions. Memungkinkan untuk menentukan opsi tambahan saat menyimpan proyek ke CSV."
type: docs
weight: 1980
url: /id/net/aspose.tasks.saving/csvoptions/
---
## CsvOptions class

Mengizinkan untuk menentukan opsi tambahan saat menyimpan proyek ke CSV.

```csharp
public class CsvOptions : SimpleSaveOptions
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [CsvOptions](csvoptions/)() | Menginisialisasi instance baru dari kelas `CsvOptions` yang dapat digunakan untuk menyimpan proyek dalam format CSV. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [DataCategory](../../aspose.tasks.saving/csvoptions/datacategory/) { get; set; } | Mendapatkan atau mengatur kategori data yang akan disimpan. |
| [Encoding](../../aspose.tasks.saving/csvoptions/encoding/) { get; set; } | Mendapatkan atau mengatur enkoding untuk menyimpan CSV. |
| [IncludeHeaders](../../aspose.tasks.saving/csvoptions/includeheaders/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah menyertakan header atau tidak (nilai default adalah TRUE). |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Mendapatkan atau mengatur format di mana dokumen akan disimpan jika objek opsi penyimpanan ini digunakan. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Mendapatkan atau mengatur pembanding untuk mengurutkan tugas pada diagram Gantt dan diagram Lembar Tugas. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Mendapatkan atau mengatur kondisi yang digunakan untuk memfilter tugas yang dirender pada diagram Gantt, Lembar Tugas, dan Penggunaan Tugas. |
| [TextDelimiter](../../aspose.tasks.saving/csvoptions/textdelimiter/) { get; set; } | Mendapatkan atau mengatur pembatas teks. |
| [View](../../aspose.tasks.saving/csvoptions/view/) { get; set; } | Mendapatkan atau mengatur daftar kolom tampilan ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)) untuk disimpan dalam format XLSX. Jika tidak diatur, maka kolom default akan disimpan. |

## Contoh

Menampilkan cara menggunakan &lt;see cref="Aspose.Tasks.Saving.CsvOptions" /&gt; untuk menyimpan proyek sebagai file CSV.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
var options = new CsvOptions
{
    DataCategory = DataCategory.Resources,
    TextDelimiter = CsvTextDelimiter.Semicolon,
    Encoding = Encoding.Unicode, IncludeHeaders = true
};

project.Save(OutDir + "WorkWithCsvOptions_out.csv", options);
```

Menampilkan cara menggunakan &lt;see cref=\"Aspose.Tasks.Saving.CsvOptions\" /&gt; untuk mengambil kolom dari Gantt Chart default dan

```csharp
// menyimpannya ke file CSV.
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

CsvOptions options = new CsvOptions();
options.TextDelimiter = CsvTextDelimiter.Tab;

var view = project.DefaultView;
options.View = ProjectView.GetDefaultGanttChartView();
options.View.Columns.Clear();

foreach (var t in view.Table.TableFields)
{
    var columnTitle = string.IsNullOrEmpty(t.Title) ? FieldHelper.GetDefaultFieldTitle(t.Field) : t.Title;
    options.View.Columns.Add(new GanttChartColumn(columnTitle, 10, t.Field));
}

project.Save(OutDir + "CustomizeViewForCsvOptions_out.csv", options);
```

### Lihat Juga

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


