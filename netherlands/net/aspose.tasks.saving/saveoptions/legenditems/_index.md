---
title: "SaveOptions.LegendItems"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "SaveOptions eigenschap. Geeft een array van PageLegendItem die definiëren welke balken moeten worden gerenderd in de paginalegend. Als null, worden de standaarditems gerenderd."
type: docs
weight: 90
url: /nl/net/aspose.tasks.saving/saveoptions/legenditems/
---
## SaveOptions.LegendItems property

Haalt op of stelt een array van PageLegendItem in die bepaalt welke balken in de paginalegenda moeten worden gerenderd. Indien null, worden de standaarditems gerenderd.

```csharp
public PageLegendItem[] LegendItems { get; set; }
```

## Opmerkingen

Is alleen van toepassing wanneer de Gantt‑chartweergave wordt gerenderd.

## Voorbeelden

Toont hoe taakbalken in de paginalegend van een Gantt-diagram aangepast kunnen worden.

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

### Zie ook

* class [PageLegendItem](../../../aspose.tasks.visualization/pagelegenditem/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


