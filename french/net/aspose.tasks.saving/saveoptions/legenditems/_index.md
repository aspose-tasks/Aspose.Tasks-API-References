---
title: "SaveOptions.LegendItems"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété SaveOptions. Obtient ou définit un tableau de PageLegendItem qui définit quelles barres doivent être rendues dans la légende de la page. Si null, les éléments par défaut sont rendus"
type: docs
weight: 90
url: /fr/net/aspose.tasks.saving/saveoptions/legenditems/
---
## SaveOptions.LegendItems property

Obtient ou définit un tableau de PageLegendItem qui définit quelles barres doivent être rendues dans la légende de la page. Si null, les éléments par défaut sont rendus.

```csharp
public PageLegendItem[] LegendItems { get; set; }
```

## Remarques

Ne s'applique que lorsque la vue du diagramme de Gantt est rendue.

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

* class [PageLegendItem](../../../aspose.tasks.visualization/pagelegenditem/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


