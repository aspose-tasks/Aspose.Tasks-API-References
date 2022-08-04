---
title: GanttChartView
second_title: Referencia de Aspose.Tasks para la API de .NET
description: Representa una vista de GanttChart.
type: docs
weight: 690
url: /es/net/aspose.tasks/ganttchartview/
---
## GanttChartView class

Representa una vista de GanttChart.

```csharp
public class GanttChartView : View
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [GanttChartView](ganttchartview)() | Inicializa una nueva instancia del[`GanttChartView`](../ganttchartview) clase. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AutoFilters](../../aspose.tasks/ganttchartview/autofilters) { get; } | Obtiene una lista de filtros automáticos de una vista de Diagrama de Gantt. |
| [BarRounding](../../aspose.tasks/ganttchartview/barrounding) { get; set; } | Obtiene o establece un valor que indica si las barras se redondean al día más cercano. El valor predeterminado es Verdadero. |
| [BarSize](../../aspose.tasks/ganttchartview/barsize) { get; set; } | Obtiene o establece la altura, en puntos, de las barras de Gantt en el Diagrama de Gantt. |
| [BarStyles](../../aspose.tasks/ganttchartview/barstyles) { get; } | Obtiene una lista de estilos de barra principales (comunes) de la vista Diagrama de Gantt. [`GanttBarStyle`](../../aspose.tasks.visualization/ganttbarstyle) . |
| [BottomTimescaleTier](../../aspose.tasks/ganttchartview/bottomtimescaletier) { get; set; } | Obtiene o establece la configuración del nivel de escala de tiempo inferior de la vista. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier) |
| [CustomBarStyles](../../aspose.tasks/ganttchartview/custombarstyles) { get; } | Obtiene una lista de estilos de barra personalizados específicos de tareas de la vista Diagrama de Gantt. [`GanttBarStyle`](../../aspose.tasks.visualization/ganttbarstyle) . |
| [Filter](../../aspose.tasks/view/filter) { get; set; } | Obtiene o establece un filtro utilizado en una sola vista. |
| [Gridlines](../../aspose.tasks/ganttchartview/gridlines) { get; set; } | Obtiene o establece una lista de[`Gridlines`](./gridlines) de la vista Diagrama de Gantt. |
| [Group](../../aspose.tasks/view/group) { get; set; } | Obtiene o establece un grupo de la vista única. |
| [HideRollupBarsWhenSummaryExpanded](../../aspose.tasks/ganttchartview/hiderollupbarswhensummaryexpanded) { get; set; } | Obtiene o establece un valor que indica si las barras acumulativas se ocultarán al expandir la tarea de resumen. |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter) { get; set; } | Obtiene o establece un valor que indica si Microsoft Project resalta el filtro para una sola vista. |
| [MiddleTimescaleTier](../../aspose.tasks/ganttchartview/middletimescaletier) { get; set; } | Obtiene o establece la configuración del nivel de escala de tiempo medio de la vista. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier) . |
| [Name](../../aspose.tasks/view/name) { get; set; } | Obtiene o establece el nombre de un objeto View. |
| [NonWorkingTimeColor](../../aspose.tasks/ganttchartview/nonworkingtimecolor) { get; set; } | Obtiene o establece el color del tiempo no laborable. |
| [PageInfo](../../aspose.tasks/view/pageinfo) { get; } | Obtiene una instancia del[`PageInfo`](../view/pageinfo)clase. Representa datos de configuración de página que están presentes en formato de archivo mpp. |
| [ParentProject](../../aspose.tasks/view/parentproject) { get; } | Obtiene el padre del objeto View. Solo lectura[`Project`](../project) . |
| [ProgressLines](../../aspose.tasks/ganttchartview/progresslines) { get; set; } | Obtiene o establece líneas de progreso para la vista Diagrama de Gantt. [`ProgressLines`](./progresslines) . |
| [RollUpGanttBars](../../aspose.tasks/ganttchartview/rollupganttbars) { get; set; } | Obtiene o establece un valor que indica si las barras del diagrama de Gantt se deben resumir. |
| [Screen](../../aspose.tasks/view/screen) { get; } | Obtiene el tipo de pantalla para la vista única. Solo lectura[`ViewScreen`](../viewscreen) . |
| [ShowBarSplits](../../aspose.tasks/ganttchartview/showbarsplits) { get; set; } | Obtiene o establece un valor que indica si se deben mostrar las divisiones de tareas en el diagrama de Gantt. |
| [ShowDrawings](../../aspose.tasks/ganttchartview/showdrawings) { get; set; } | Obtiene o establece un valor que indica si se deben mostrar los dibujos en el diagrama de Gantt. |
| [ShowInMenu](../../aspose.tasks/view/showinmenu) { get; set; } | Obtiene o establece un valor que indica si Microsoft Project muestra el nombre de la vista individual en las listas desplegables Vista u Otras vistas en la cinta. |
| [Table](../../aspose.tasks/view/table) { get; set; } | Obtiene o establece una tabla de la vista única. |
| [TableTextStyles](../../aspose.tasks/ganttchartview/tabletextstyles) { get; } | Obtiene una lista de estilos de texto de tabla de la vista Diagrama de Gantt. [`TableTextStyle`](../../aspose.tasks.visualization/tabletextstyle) . |
| [TextStyles](../../aspose.tasks/ganttchartview/textstyles) { get; set; } | Obtiene o establece una lista de[`TextStyle`](../../aspose.tasks.visualization/textstyle) de la vista Diagrama de Gantt. |
| [TimescaleSizePercentage](../../aspose.tasks/ganttchartview/timescalesizepercentage) { get; set; } |  |
| [TopTimescaleTier](../../aspose.tasks/ganttchartview/toptimescaletier) { get; set; } | Obtiene o establece la configuración del nivel de escala de tiempo superior de la vista. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier) . |
| [Type](../../aspose.tasks/view/type) { get; } | Obtiene el tipo de elemento en la vista única, como tareas o recursos. Solo lectura[`ItemType`](../itemtype) . |
| [Uid](../../aspose.tasks/view/uid) { get; } | Obtiene el identificador único de una vista. |
| [VisualObjectsPlacements](../../aspose.tasks/view/visualobjectsplacements) { get; } | Obtiene una colección de objetos que representan la ubicación y apariencia de[`OleObject`](../oleobject) en la vista. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [CompareTo](../../aspose.tasks/view/compareto)(View) | Compara la instancia actual con otro objeto del mismo tipo y devuelve un número entero que indica si la instancia actual precede, sigue u ocurre en la misma posición en el orden de clasificación que el otro objeto. |
| override [Equals](../../aspose.tasks/view/equals)(object) | Devuelve un valor que indica si esta instancia es igual a un objeto especificado. |
| override [GetHashCode](../../aspose.tasks/view/gethashcode)() | Devuelve un valor de código hash para la instancia del[`Resource`](../resource) clase. |

### Ver también

* class [View](../view)
* espacio de nombres [Aspose.Tasks](../../aspose.tasks)
* asamblea [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
