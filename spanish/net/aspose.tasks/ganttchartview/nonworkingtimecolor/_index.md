---
title: "GanttChartView.NonWorkingTimeColor"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad de GanttChartView. Obtiene o establece el color del tiempo no laborable"
type: docs
weight: 110
url: /es/net/aspose.tasks/ganttchartview/nonworkingtimecolor/
---
## GanttChartView.NonWorkingTimeColor property

Obtiene o establece el color del tiempo no laborable.

```csharp
public Color NonWorkingTimeColor { get; set; }
```

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

* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


