---
title: "SaveOptions.LegendItems"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad SaveOptions. Obtiene o establece una matriz de PageLegendItem que define qué barras deben renderizarse en la leyenda de la página. Si es null, se renderizan los elementos predeterminados."
type: docs
weight: 90
url: /es/net/aspose.tasks.saving/saveoptions/legenditems/
---
## SaveOptions.LegendItems property

Obtiene o establece una matriz de PageLegendItem que define qué barras deben renderizarse en la leyenda de la página. Si es null, se renderizan los elementos predeterminados.

```csharp
public PageLegendItem[] LegendItems { get; set; }
```

## Observaciones

Solo se aplica cuando se renderiza la vista de diagrama de Gantt.

## Ejemplos

Muestra cómo personalizar las barras de tareas en la leyenda de página del diagrama de Gantt.

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

### Ver también

* class [PageLegendItem](../../../aspose.tasks.visualization/pagelegenditem/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


