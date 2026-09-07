---
title: "SaveOptions.Gridlines"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti SaveOptions. Mendapatkan atau mengatur daftar Gridline yang muncul dalam tampilan proyek"
type: docs
weight: 60
url: /id/net/aspose.tasks.saving/saveoptions/gridlines/
---
## SaveOptions.Gridlines property

Mendapatkan atau mengatur daftar [`Gridline`](../../../aspose.tasks.visualization/gridline/) yang muncul dalam tampilan proyek.

```csharp
public List<Gridline> Gridlines { get; set; }
```

## Contoh

Menampilkan cara menyimpan tata letak ke file terpisah.

```csharp
var project = new Project(DataDir + "Homemoveplan.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Png);
options.StartDate = project.Get(Prj.StartDate).AddDays(-3);
options.EndDate = project.Get(Prj.FinishDate);
options.MarkCriticalTasks = true;
options.LegendDrawingOptions = LegendDrawingOptions.NoLegend;
options.FontSettings.DefaultFontName = "Segoe UI Black";
options.FontSettings.UseProjectDefaultFont = false;
options.PageSize = PageSize.Letter;

options.Gridlines = new List<Gridline>();

var gridline = new Gridline { GridlineType = GridlineType.GanttRow, Color = Color.CornflowerBlue, Pattern = LinePattern.Dashed };
options.Gridlines.Add(gridline);

project.Save(OutDir + "PrintProjectPagesToSeparateFiles1_out.png", options);

// Simpan tata letak proyek ke file terpisah
options.RenderToSinglePage = false;
project.Save(OutDir + "PrintProjectPagesToSeparateFiles2_out.png", options);
```

### Lihat Juga

* class [Gridline](../../../aspose.tasks.visualization/gridline/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


