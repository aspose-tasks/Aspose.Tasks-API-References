---
title: "Classe PageLegendItem"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Visualization.PageLegendItem. Rappresenta un elemento della legenda di pagina del diagramma di Gantt"
type: docs
weight: 3220
url: /it/net/aspose.tasks.visualization/pagelegenditem/
---
## PageLegendItem class

Rappresenta un elemento della legenda di pagina del diagramma di Gantt.

```csharp
public sealed class PageLegendItem
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [PageLegendItem](pagelegenditem/)(BarItemType, string) | Inizializza una nuova istanza della classe `PageLegendItem`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ItemType](../../aspose.tasks.visualization/pagelegenditem/itemtype/) { get; } | Ottiene il tipo dell'elemento. |
| [Title](../../aspose.tasks.visualization/pagelegenditem/title/) { get; } | Ottiene l'etichetta di testo dell'elemento. |

## Esempi

Mostra come personalizzare le barre delle attività nella legenda di pagina del diagramma di Gantt.

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

### Vedi anche

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


