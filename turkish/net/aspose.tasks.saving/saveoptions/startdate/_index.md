---
title: "SaveOptions.StartDate"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "SaveOptions özelliği. Render etmeye başlanacak tarihi alır veya ayarlar."
type: docs
weight: 170
url: /tr/net/aspose.tasks.saving/saveoptions/startdate/
---
## SaveOptions.StartDate property

Renderlamaya başlanacak tarihi alır veya ayarlar.

```csharp
public DateTime StartDate { get; set; }
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

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


