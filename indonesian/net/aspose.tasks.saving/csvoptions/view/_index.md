---
title: "CsvOptions.View"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti CsvOptions. Mendapatkan atau mengatur daftar kolom tampilan GanttChartColumn untuk disimpan dalam format XLSX. Jika tidak diatur, maka kolom default akan disimpan"
type: docs
weight: 60
url: /id/net/aspose.tasks.saving/csvoptions/view/
---
## CsvOptions.View property

Mendapatkan atau mengatur daftar kolom tampilan ([`GanttChartColumn`](../../../aspose.tasks.visualization/ganttchartcolumn/)) untuk disimpan dalam format XLSX. Jika tidak diatur, maka kolom default akan disimpan.

```csharp
public ProjectView View { get; set; }
```

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

* class [ProjectView](../../../aspose.tasks.visualization/projectview/)
* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


