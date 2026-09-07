---
title: "SaveOptions.StartDate"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti SaveOptions. Mendapatkan atau mengatur tanggal mulai rendering"
type: docs
weight: 170
url: /id/net/aspose.tasks.saving/saveoptions/startdate/
---
## SaveOptions.StartDate property

Mendapatkan atau mengatur tanggal mulai merender.

```csharp
public DateTime StartDate { get; set; }
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

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


