---
title: "SaveOptions.MarkCriticalTasks"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "SaveOptions özelliği. Kritik görevlerin kırmızı renkte gösterilip gösterilmeyeceğini belirten bir değeri alır veya ayarlar. Varsayılan değer FALSE'tur."
type: docs
weight: 100
url: /tr/net/aspose.tasks.saving/saveoptions/markcriticaltasks/
---
## SaveOptions.MarkCriticalTasks property

Kritik görevlerin kırmızı renkte gösterilip gösterilmeyeceğini belirten bir değeri alır veya ayarlar (Varsayılan değer FALSE'tır).

```csharp
public bool MarkCriticalTasks { get; set; }
```

## Örnekler

Kritik görevlerin görüntü dosyası formatlarında kaydedilirken nasıl yazdırılacağını gösterir.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Png)
{
    StartDate = project.Get(Prj.StartDate).AddDays(-3),
    EndDate = project.Get(Prj.FinishDate),
    MarkCriticalTasks = true,
    LegendDrawingOptions = LegendDrawingOptions.NoLegend,
    Gridlines = new List<Gridline>()
};

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


