---
title: "Clase GanttChartView"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.GanttChartView. Representa una vista GanttChart"
type: docs
weight: 710
url: /es/net/aspose.tasks/ganttchartview/
---
## GanttChartView class

Representa una vista GanttChart.

```csharp
public class GanttChartView : View
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [GanttChartView](ganttchartview/)() | Inicializa una nueva instancia de la clase `GanttChartView`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AutoFilters](../../aspose.tasks/ganttchartview/autofilters/) { get; } | Obtiene una lista de filtros automáticos de una vista Gantt Chart. |
| [BarRounding](../../aspose.tasks/ganttchartview/barrounding/) { get; set; } | Obtiene o establece un valor que indica si las barras se redondean al día más cercano. El valor predeterminado es True. |
| [BarSize](../../aspose.tasks/ganttchartview/barsize/) { get; set; } | Obtiene o establece la altura, en puntos, de las barras Gantt en el Gantt Chart. |
| [BarStyles](../../aspose.tasks/ganttchartview/barstyles/) { get; } | Obtiene una lista de estilos de barra padre (comunes) de la vista Gantt Chart. [`GanttBarStyle`](../../aspose.tasks.visualization/ganttbarstyle/). |
| [BottomTimescaleTier](../../aspose.tasks/ganttchartview/bottomtimescaletier/) { get; set; } | Obtiene o establece la configuración del nivel inferior de la escala de tiempo de la vista. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/) |
| [CustomBarStyles](../../aspose.tasks/ganttchartview/custombarstyles/) { get; } | Obtiene una lista de estilos de barra personalizados específicos de tareas de la vista Gantt Chart. [`GanttBarStyle`](../../aspose.tasks.visualization/ganttbarstyle/). |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | Obtiene o establece un filtro utilizado en una vista única. |
| [Gridlines](../../aspose.tasks/ganttchartview/gridlines/) { get; set; } | Obtiene o establece una lista de [`Gridlines`](./gridlines/) de la vista Gantt Chart. |
| [Group](../../aspose.tasks/view/group/) { get; set; } | Obtiene o establece un grupo de la vista única. |
| [HideRollupBarsWhenSummaryExpanded](../../aspose.tasks/ganttchartview/hiderollupbarswhensummaryexpanded/) { get; set; } | Obtiene o establece un valor que indica si las barras de consolidación se ocultarán al expandir la tarea resumen. |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | Obtiene o establece un valor que indica si Microsoft Project resalta el filtro para una vista única. |
| [MiddleTimescaleTier](../../aspose.tasks/ganttchartview/middletimescaletier/) { get; set; } | Obtiene o establece la configuración del nivel medio de la escala de tiempo de la vista. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/). |
| [Name](../../aspose.tasks/view/name/) { get; set; } | Obtiene o establece el nombre de un objeto View. |
| [NonWorkingTimeColor](../../aspose.tasks/ganttchartview/nonworkingtimecolor/) { get; set; } | Obtiene o establece el color del tiempo no laborable. |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | Obtiene una instancia de la clase [`PageInfo`](../view/pageinfo/). Representa los datos de configuración de página que están presentes en el formato de archivo mpp. |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | Obtiene el padre del objeto View. Solo lectura [`Project`](../project/). |
| [ProgressLines](../../aspose.tasks/ganttchartview/progresslines/) { get; set; } | Obtiene o establece líneas de progreso para la vista Gantt Chart. [`ProgressLines`](./progresslines/). |
| [RollUpGanttBars](../../aspose.tasks/ganttchartview/rollupganttbars/) { get; set; } | Obtiene o establece un valor que indica si las barras en el Gantt Chart deben consolidarse. |
| [Screen](../../aspose.tasks/view/screen/) { get; } | Obtiene el tipo de pantalla para la vista única. Solo lectura [`ViewScreen`](../viewscreen/). |
| [ShowBarSplits](../../aspose.tasks/ganttchartview/showbarsplits/) { get; set; } | Obtiene o establece un valor que indica si se deben mostrar divisiones de tareas en el Gantt Chart. |
| [ShowDrawings](../../aspose.tasks/ganttchartview/showdrawings/) { get; set; } | Obtiene o establece un valor que indica si se deben mostrar dibujos en el Gantt Chart. |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | Obtiene o establece un valor que indica si Microsoft Project muestra el nombre de la vista única en las listas desplegables Vista u Otras Vistas en la cinta de opciones. |
| [Table](../../aspose.tasks/view/table/) { get; set; } | Obtiene o establece una tabla de la vista única. |
| [TableTextStyles](../../aspose.tasks/ganttchartview/tabletextstyles/) { get; } | Obtiene una lista de estilos de texto de tabla de la vista Gantt Chart. [`TableTextStyle`](../../aspose.tasks.visualization/tabletextstyle/). |
| [TextStyles](../../aspose.tasks/ganttchartview/textstyles/) { get; set; } | Obtiene o establece una lista de [`TextStyle`](../../aspose.tasks.visualization/textstyle/) de la vista Gantt Chart. |
| [TimescaleSizePercentage](../../aspose.tasks/ganttchartview/timescalesizepercentage/) { get; set; } |  |
| [TopTimescaleTier](../../aspose.tasks/ganttchartview/toptimescaletier/) { get; set; } | Obtiene o establece la configuración del nivel superior de la escala de tiempo de la vista. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/). |
| [Type](../../aspose.tasks/view/type/) { get; } | Obtiene el tipo de elemento en la vista única, como tareas o recursos. Solo lectura [`ItemType`](../itemtype/). |
| [Uid](../../aspose.tasks/view/uid/) { get; } | Obtiene el identificador único de una vista. |
| [VisualObjectsPlacements](../../aspose.tasks/view/visualobjectsplacements/) { get; } | Obtiene una colección de objetos que representan la ubicación y apariencia de [`OleObject`](../oleobject/) en la vista. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [CompareTo](../../aspose.tasks/view/compareto/)(View) | Compara la instancia actual con otro objeto del mismo tipo y devuelve un entero que indica si la instancia actual precede, sigue o se encuentra en la misma posición en el orden de clasificación que el otro objeto. |
| override [Equals](../../aspose.tasks/view/equals/)(object) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| override [GetHashCode](../../aspose.tasks/view/gethashcode/)() | Devuelve un valor de código hash para la instancia de la clase [`Resource`](../resource/). |

## Ejemplos

Muestra cómo modificar los niveles de escala de tiempo.

```csharp
var project = new Project();

// Inicializar vista Gantt Chart
var view = new GanttChartView
{
    TopTimescaleTier = new TimescaleTier(),
    MiddleTimescaleTier = new TimescaleTier(),
    BottomTimescaleTier = new TimescaleTier()
};

// establecer el recuento de escala de tiempo
view.TopTimescaleTier.Count = 2;
view.TopTimescaleTier.Unit = TimescaleUnit.Quarters;
view.TopTimescaleTier.Label = DateLabel.QuarterQQyy;
view.TopTimescaleTier.ShowTicks = false;

view.MiddleTimescaleTier.Count = 2;
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
view.MiddleTimescaleTier.ShowTicks = false;

view.BottomTimescaleTier.Unit = TimescaleUnit.Days;
view.BottomTimescaleTier.Label = DateLabel.DayDdd;
view.BottomTimescaleTier.Count = 2;
view.BottomTimescaleTier.ShowTicks = false;

// agregar vista Gantt Chart al proyecto
project.Views.Add(view);

// agregar algunos datos de prueba al proyecto
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");
task1.Set(Tsk.Duration, task1.ParentProject.GetDuration(24, TimeUnitType.Hour));
task2.Set(Tsk.Duration, task1.ParentProject.GetDuration(40, TimeUnitType.Hour));

// Utilice la opción 'Timescale.DefinedInView' para renderizar escalas de tiempo usando la configuración de escala de tiempo que hemos establecido (view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier).
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    StartDate = DateTime.Now.AddDays(-30),
    EndDate = DateTime.Now.AddDays(30)
};

project.Save(OutDir + "WorkWithTimescaleTier_out.pdf", pdfSaveOptions);
```

### Ver también

* class [View](../view/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


