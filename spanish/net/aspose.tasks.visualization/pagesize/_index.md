---
title: "Enumeración PageSize"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.Visualization.PageSize enum. Especifica el tamaño de página."
type: docs
weight: 3250
url: /es/net/aspose.tasks.visualization/pagesize/
---
## PageSize enumeration

Especifica el tamaño de página.

```csharp
public enum PageSize
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Letter | `0` | El tamaño de la página Letter en puntos es 792 × 612. |
| Ledger | `1` | El tamaño de la página Ledger en puntos es 1224 × 792. |
| A0 | `2` | El tamaño de la página A0 en puntos es 3371 × 2384. |
| A1 | `3` | El tamaño de la página A1 en puntos es 2384 × 1685. |
| A2 | `4` | El tamaño de la página A2 en puntos es 1684 × 1190. |
| A3 | `5` | El tamaño de la página A3 en puntos es 1190 × 842. |
| A4 | `6` | El tamaño de la página A4 en puntos es 842 × 595. |
| DefinedInView | `7` | Utilice el tamaño de página definido en [`PageSettings`](../pagesettings/) de la Vista (View.PageInfo.PageSettings). |

## Ejemplos

Muestra cómo establecer un valor que indica que las subtareas en la barra de la tarea resumen deben consolidarse.

```csharp
var project = new Project(DataDir + "Project2.mpp");

project.DisplayOptions.ShowProjectSummaryTask = true;
project.Set(Prj.ShowProjectSummaryTask, true);

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
    FitContent = true,
    RollUpGanttBars = true,

    // O
    // options.RollUpGanttBars = false;
    // DrawNonWorkingTime = true,
    PageSize = PageSize.A3
};

project.Save(OutDir + "RenderGanttChartWithBarsRolledUp_out.pdf", options);
```

### Ver también

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


