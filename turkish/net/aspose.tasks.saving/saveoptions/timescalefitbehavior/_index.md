---
title: "SaveOptions.TimescaleFitBehavior"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "SaveOptions özelliği. Zaman ölçeğinin sağ ucunun sayfa sonu ile nasıl hizalanacağını tanımlayan bir davranışı alır veya ayarlar."
type: docs
weight: 210
url: /tr/net/aspose.tasks.saving/saveoptions/timescalefitbehavior/
---
## SaveOptions.TimescaleFitBehavior property

Zaman ölçeğinin sağ ucunun sayfa sonu ile nasıl hizalanacağını tanımlayan davranışı alır veya ayarlar.

```csharp
public TimescaleFitBehavior TimescaleFitBehavior { get; set; }
```

## Örnekler

TimescaleFitBehavior'ı kullanarak Gantt şemasının zaman ölçeğini son sayfanın sonuna sığdırmayı gösterir.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.DefaultView as GanttChartView;

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.PageSize = PageSize.A4;
saveOptions.StartDate = project.StartDate;
saveOptions.EndDate = project.FinishDate;
saveOptions.ViewSettings = view;
saveOptions.TimescaleFitBehavior = TimescaleFitBehavior.ScaleToEndOfPage;

project.Save(OutDir + "WorkWithPageSizeDefinedInView_out.pdf", saveOptions);
```

### Ayrıca Bakınız

* enum [TimescaleFitBehavior](../../../aspose.tasks.visualization/timescalefitbehavior/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


