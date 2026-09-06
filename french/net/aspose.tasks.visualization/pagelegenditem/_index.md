---
title: "Classe PageLegendItem"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.Visualization.PageLegendItem. Représente un élément de la légende de page du diagramme de Gantt"
type: docs
weight: 3220
url: /fr/net/aspose.tasks.visualization/pagelegenditem/
---
## PageLegendItem class

Représente un élément de la légende de page du diagramme de Gantt.

```csharp
public sealed class PageLegendItem
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [PageLegendItem](pagelegenditem/)(BarItemType, string) | Initialise une nouvelle instance de la classe `PageLegendItem`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [ItemType](../../aspose.tasks.visualization/pagelegenditem/itemtype/) { get; } | Obtient le type de l'élément. |
| [Title](../../aspose.tasks.visualization/pagelegenditem/title/) { get; } | Obtient le libellé texte de l'élément. |

## Exemples

Montre comment personnaliser les barres de tâches dans la légende de page du diagramme de Gantt.

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

### Voir aussi

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


