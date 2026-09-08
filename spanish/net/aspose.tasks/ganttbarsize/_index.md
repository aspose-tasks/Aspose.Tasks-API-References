---
title: "Enum GanttBarSize"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enum Aspose.Tasks.GanttBarSize. Especifica la altura de una barra en puntos."
type: docs
weight: 700
url: /es/net/aspose.tasks/ganttbarsize/
---
## GanttBarSize enumeration

Especifica la altura de una barra en puntos.

```csharp
public enum GanttBarSize
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| BarSize6 | `0` | Tamaño de barra 6 puntos. |
| BarSize8 | `1` | Tamaño de barra 8 puntos. |
| BarSize10 | `2` | Tamaño de barra 10 puntos. |
| BarSize12 | `3` | Tamaño de barra 12 puntos. |
| BarSize14 | `4` | Tamaño de barra 14 puntos. |
| BarSize18 | `5` | Tamaño de barra 18 puntos. |
| BarSize24 | `6` | Tamaño de barra 24 puntos. |

## Ejemplos

Muestra cómo establecer algunas propiedades útiles de la vista de diagrama de Gantt.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[0];

// establece un valor que indica si las barras se redondean al día más cercano
view.BarRounding = false;
// establece la altura, en puntos, de las barras de Gantt en el diagrama de Gantt
view.BarSize = GanttBarSize.BarSize24;
// establece un valor que indica si las barras de consolidación se ocultarán al expandir la tarea resumida
view.HideRollupBarsWhenSummaryExpanded = true;
// establece el color del tiempo no laborable
view.NonWorkingTimeColor = Color.Azure;
// establece un valor que indica si las barras en el diagrama de Gantt deben consolidarse
view.RollUpGanttBars = true;
// establece un valor que indica si se deben mostrar las divisiones de tareas en el diagrama de Gantt
view.ShowBarSplits = true;
// establece un valor que indica si se deben mostrar los dibujos en el diagrama de Gantt
view.ShowDrawings = true;
// establece un porcentaje para reducir o ampliar el espaciado entre unidades en el nivel de escala de tiempo
view.TimescaleSizePercentage = 10;

project.Save(OutDir + "WorkWithGanttChartViews_out.pdf", SaveFileFormat.Pdf);
```

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


