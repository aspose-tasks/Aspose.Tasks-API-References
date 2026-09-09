---
title: "SaveOptions.Gridlines"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "SaveOptions özelliği. Proje görünümünde görünen Gridline'ların bir listesini alır veya ayarlar."
type: docs
weight: 60
url: /tr/net/aspose.tasks.saving/saveoptions/gridlines/
---
## SaveOptions.Gridlines property

Proje görünümünde görünen [`Gridline`](../../../aspose.tasks.visualization/gridline/) listesini alır veya ayarlar.

```csharp
public List<Gridline> Gridlines { get; set; }
```

## Örnekler

Düzeni ayrı dosyalara kaydetmenin nasıl yapılacağını gösterir.

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

// Proje düzenini ayrı dosyalara kaydet
options.RenderToSinglePage = false;
project.Save(OutDir + "PrintProjectPagesToSeparateFiles2_out.png", options);
```

### Ayrıca Bakınız

* class [Gridline](../../../aspose.tasks.visualization/gridline/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


