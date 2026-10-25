---
title: "Enum TimescaleFitBehavior"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enum Aspose.Tasks.Visualization.TimescaleFitBehavior. Representa un comportamiento usado para alinear el área de escala de tiempo con el ancho de la página"
type: docs
weight: 3440
url: /es/net/aspose.tasks.visualization/timescalefitbehavior/
---
## TimescaleFitBehavior enumeration

Representa un comportamiento utilizado para alinear el área de escala de tiempo con el ancho de página.

```csharp
public enum TimescaleFitBehavior
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| DefinedInView | `0` | La sección del calendario se renderiza según la propiedad View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage de la vista renderizada. |
| NoScaleToEndDate | `1` | La sección del calendario se renderiza exactamente hasta EndDate, incluso si hay un espacio vacío en una página. |
| NoScaleToEndOfPage | `2` | La sección del calendario se renderiza hasta el final (lado derecho) de la última página. Por lo tanto, la última fecha renderizada puede exceder EndDate. |
| ScaleToEndOfPage | `3` | El motor de renderizado intentará alinear las fechas de modo que EndDate quede alineado con el final (lado derecho) de la última página. Corresponde a la opción habilitada de "Page Setup \ View \ Fit timescale to end of page" de MS Project. |

## Ejemplos

Muestra cómo usar TimescaleFitBehavior para que la escala de tiempo del diagrama de Gantt se ajuste al final de la última página.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.DefaultView as GanttChartView;

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.PageSize = PageSize.A4;
saveOptions.StartDate = project.StartDate;
saveOptions.EndDate = project.FinishDate;
saveOptions.ViewSettings = view;
saveOptions.TimescaleFitBehavior = TimescaleFitBehavior.ScaleToEndOfPage;

project.Save(OutDir + "WorkWithPageSizeDefinedInView_out.pdf", saveOptions);
```

### Ver también

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


