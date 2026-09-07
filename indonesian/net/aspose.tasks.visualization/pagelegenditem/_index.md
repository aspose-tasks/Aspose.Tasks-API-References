---
title: "Kelas PageLegendItem"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Visualization.PageLegendItem. Mewakili item legenda halaman pada diagram Gantt"
type: docs
weight: 3220
url: /id/net/aspose.tasks.visualization/pagelegenditem/
---
## PageLegendItem class

Mewakili item legenda halaman pada diagram Gantt.

```csharp
public sealed class PageLegendItem
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [PageLegendItem](pagelegenditem/)(BarItemType, string) | Menginisialisasi instance baru dari kelas `PageLegendItem`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [ItemType](../../aspose.tasks.visualization/pagelegenditem/itemtype/) { get; } | Mendapatkan tipe item. |
| [Title](../../aspose.tasks.visualization/pagelegenditem/title/) { get; } | Mendapatkan label teks dari item. |

## Contoh

Menampilkan cara menyesuaikan batang tugas dalam legenda halaman pada diagram Gantt.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.StartDate = project.StartDate;
pdfSaveOptions.EndDate = project.FinishDate;
pdfSaveOptions.PageSize = PageSize.A4;
pdfSaveOptions.LegendDrawingOptions = LegendDrawingOptions.OnEveryPage;
pdfSaveOptions.ViewSettings = project.Views.GetByName("&Gantt Chart");

pdfSaveOptions.LegendItems = new PageLegendItem[]
{
    new PageLegendItem(BarItemType.Task, "Task"),
    new PageLegendItem(BarItemType.ExternalMilestone, "External Milestone"),
    new PageLegendItem(BarItemType.SummaryRollup, "Summary Rollup"),
    new PageLegendItem(BarItemType.InactiveTask, "Inactive Task"),
    new PageLegendItem(BarItemType.ManualSummary, "Manual Summary")
};

project.Save(OutDir + "CustomizePageLegendItems_out.pdf", pdfSaveOptions);
```

### Lihat Juga

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


