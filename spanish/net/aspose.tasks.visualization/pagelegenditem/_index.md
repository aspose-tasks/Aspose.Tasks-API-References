---
title: "Clase PageLegendItem"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Visualization.PageLegendItem. Representa un elemento de la leyenda de página del diagrama de Gantt"
type: docs
weight: 3220
url: /es/net/aspose.tasks.visualization/pagelegenditem/
---
## PageLegendItem class

Representa un elemento de la leyenda de página del diagrama de Gantt.

```csharp
public sealed class PageLegendItem
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [PageLegendItem](pagelegenditem/)(BarItemType, string) | Inicializa una nueva instancia de la clase `PageLegendItem`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ItemType](../../aspose.tasks.visualization/pagelegenditem/itemtype/) { get; } | Obtiene el tipo del elemento. |
| [Title](../../aspose.tasks.visualization/pagelegenditem/title/) { get; } | Obtiene la etiqueta de texto del elemento. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


