---
title: "SaveOptions.LegendItems"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "SaveOptions-Eigenschaft. Gibt ein Array von PageLegendItem zurück oder legt es fest, das definiert, welche Balken in der Seitenlegende gerendert werden sollen. Wenn null, werden die Standardelemente gerendert."
type: docs
weight: 90
url: /de/net/aspose.tasks.saving/saveoptions/legenditems/
---
## SaveOptions.LegendItems property

Liest ein Array von PageLegendItem aus oder legt es fest, das definiert, welche Balken in der Seitenlegende gerendert werden sollen. Wenn null, werden die Standard‑Elemente gerendert.

```csharp
public PageLegendItem[] LegendItems { get; set; }
```

## Hinweise

Gilt nur, wenn die Gantt‑Diagrammansicht gerendert wird.

## Beispiele

Zeigt, wie Aufgabenbalken in der Seitenlegende des Gantt-Diagramms angepasst werden können.

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

### Siehe auch

* class [PageLegendItem](../../../aspose.tasks.visualization/pagelegenditem/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


