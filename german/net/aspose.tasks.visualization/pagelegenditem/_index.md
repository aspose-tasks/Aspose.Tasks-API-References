---
title: "Klasse PageLegendItem"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "Aspose.Tasks.Visualization.PageLegendItem Klasse. Stellt ein Element der Seitenlegende des Gantt-Diagramms dar"
type: docs
weight: 3220
url: /de/net/aspose.tasks.visualization/pagelegenditem/
---
## PageLegendItem class

Stellt ein Element der Seitenlegende des Gantt-Diagramms dar.

```csharp
public sealed class PageLegendItem
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [PageLegendItem](pagelegenditem/)(BarItemType, string) | Initialisiert eine neue Instanz der `PageLegendItem` Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [ItemType](../../aspose.tasks.visualization/pagelegenditem/itemtype/) { get; } | Liefert den Typ des Elements. |
| [Title](../../aspose.tasks.visualization/pagelegenditem/title/) { get; } | Liefert das Textlabel des Elements. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


