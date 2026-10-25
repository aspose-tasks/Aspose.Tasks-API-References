---
title: "Enum PageSize"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.Visualization.PageSize enum. Sayfa boyutunu belirtir."
type: docs
weight: 3250
url: /tr/net/aspose.tasks.visualization/pagesize/
---
## PageSize enumeration

Sayfa boyutunu belirtir.

```csharp
public enum PageSize
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Letter | `0` | Letter sayfasının boyutu puan cinsinden 792 × 612'dir. |
| Ledger | `1` | Ledger sayfasının boyutu puan cinsinden 1224 × 792'dir. |
| A0 | `2` | A0 sayfasının boyutu puan cinsinden 3371 × 2384'tür. |
| A1 | `3` | A1 sayfasının boyutu puan cinsinden 2384 × 1685'tir. |
| A2 | `4` | A2 sayfasının boyutu puan cinsinden 1684 × 1190'tir. |
| A3 | `5` | A3 sayfasının boyutu puan cinsinden 1190 × 842'dir. |
| A4 | `6` | A4 sayfasının boyutu puan cinsinden 842 × 595'tir. |
| DefinedInView | `7` | Görünüm'ün [`PageSettings`](../pagesettings/) içinde tanımlanan sayfa boyutunu kullanın (View.PageInfo.PageSettings). |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


