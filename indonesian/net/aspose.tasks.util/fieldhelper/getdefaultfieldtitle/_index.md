---
title: "FieldHelper.GetDefaultFieldTitle"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode FieldHelper. Mengembalikan judul default dari field tertentu."
type: docs
weight: 10
url: /id/net/aspose.tasks.util/fieldhelper/getdefaultfieldtitle/
---
## FieldHelper.GetDefaultFieldTitle method

Mengembalikan judul default dari bidang spesifik.

```csharp
public static string GetDefaultFieldTitle(Field field)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| bidang | Bidang | Field untuk mendapatkan judul default. |

### Nilai Kembali

Judul default dari bidang tertentu jika bidang tersebut dapat ditampilkan dalam tampilan MS Project, null jika tidak.

## Contoh

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

* enum [Field](../../../aspose.tasks/field/)
* class [FieldHelper](../)
* namespace [Aspose.Tasks.Util](../../fieldhelper/)
* assembly [Aspose.Tasks](../../../)


