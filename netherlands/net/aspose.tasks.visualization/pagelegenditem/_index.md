---
title: "Klasse PageLegendItem"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Visualization.PageLegendItem klasse. Vertegenwoordigt een item van de paginalegend van een Gantt-diagram"
type: docs
weight: 3220
url: /nl/net/aspose.tasks.visualization/pagelegenditem/
---
## PageLegendItem class

Stelt een item van de paginalegende van een Gantt‑diagram voor.

```csharp
public sealed class PageLegendItem
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [PageLegendItem](pagelegenditem/)(BarItemType, string) | Initialiseert een nieuw exemplaar van de `PageLegendItem` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [ItemType](../../aspose.tasks.visualization/pagelegenditem/itemtype/) { get; } | Haalt het type van het item op. |
| [Title](../../aspose.tasks.visualization/pagelegenditem/title/) { get; } | Haalt het tekstlabel van het item op. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


