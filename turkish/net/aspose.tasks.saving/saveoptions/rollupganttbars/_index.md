---
title: "SaveOptions.RollUpGanttBars"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "SaveOptions özelliği. Özet görev çubuğundaki alt görevlerin işaretlenip işaretlenmeyeceğini belirten bir değeri alır veya ayarlar. Alt görevler için Rollup alanı, alt görev Gantt çubuklarıyla ilgili bilgilerin özet görev çubuğuna toplanıp toplanmayacağını gösterir. Özet görevler için Rollup alanı, özet görev çubuğunun toplanmış çubukları gösterip göstermediğini belirtir. Alt görevlerin onlara toplanabilmesi için özet görevlerde Rollup alanının Yes olarak ayarlanmış olması gerekir."
type: docs
weight: 160
url: /tr/net/aspose.tasks.saving/saveoptions/rollupganttbars/
---
## SaveOptions.RollUpGanttBars property

Özet görev çubuğundaki alt görevlerin işaretlenip işaretlenmeyeceğini gösteren bir değeri alır veya ayarlar. Alt görevler için Rollup alanı, alt görev Gantt çubuklarındaki bilgilerin özet görev çubuğuna toplanıp toplanmayacağını gösterir. Özet görevler için Rollup alanı, özet görev çubuğunun toplanmış çubukları gösterip göstermediğini belirtir. Alt görevlere toplanabilmesi için özet görevlerin Rollup alanının Evet olarak ayarlanmış olması gerekir.

```csharp
public bool RollUpGanttBars { get; set; }
```

## Açıklamalar

Yalnızca Gantt şeması görünümü render edildiğinde uygulanır.

## Örnekler

Özet görev çubuğundaki alt görevlerin toplanması gerektiğini gösteren bir değerin nasıl ayarlanacağını gösterir.

```csharp
var project = new Project(DataDir + "Project2.mpp");

project.DisplayOptions.ShowProjectSummaryTask = true;
project.Set(Prj.ShowProjectSummaryTask, true);

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
    FitContent = true,
    RollUpGanttBars = true,

    // VEYA
    // options.RollUpGanttBars = false;
    // DrawNonWorkingTime = true,
    PageSize = PageSize.A3
};

project.Save(OutDir + "RenderGanttChartWithBarsRolledUp_out.pdf", options);
```

### Ayrıca Bakınız

* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


