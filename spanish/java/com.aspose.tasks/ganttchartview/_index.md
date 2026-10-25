---
title: "GanttChartView"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa una vista de GanttChart."
type: docs
weight: 112
url: /es/java/com.aspose.tasks/ganttchartview/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.View](../../com.aspose.tasks/view)

**All Implemented Interfaces:**
com.aspose.tasks.ITimescaledView
```
public class GanttChartView extends View implements ITimescaledView
```

Representa una vista de GanttChart.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [GanttChartView()](#GanttChartView--) | Inicializa una nueva instancia de la clase [GanttChartView](../../com.aspose.tasks/ganttchartview). |
## Métodos

| Método | Descripción |
| --- | --- |
| [getAutoFilters()](#getAutoFilters--) | Obtiene una lista de filtros automáticos de una vista de diagrama de Gantt. |
| [getBarRounding()](#getBarRounding--) | Obtiene un valor que indica si las barras se redondean al día más cercano. |
| [getBarSize()](#getBarSize--) | Obtiene la altura, en puntos, de las barras de Gantt en el diagrama de Gantt. |
| [getBarStyles()](#getBarStyles--) | Obtiene una lista de estilos de barra padre (común) de la vista de diagrama de Gantt. |
| [getBottomTimescaleTier()](#getBottomTimescaleTier--) | Obtiene la configuración del nivel inferior de la escala de tiempo de la vista. |
| [getCustomBarStyles()](#getCustomBarStyles--) | Obtiene una lista de estilos de barra personalizados específicos de tarea de la vista de diagrama de Gantt. |
| [getGridlines()](#getGridlines--) | Obtiene una lista de `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) de la vista de diagrama de Gantt. |
| [getHideRollupBarsWhenSummaryExpanded()](#getHideRollupBarsWhenSummaryExpanded--) | Obtiene un valor que indica si las barras de consolidación se ocultarán al expandir la tarea resumen. |
| [getMiddleTimescaleTier()](#getMiddleTimescaleTier--) | Obtiene la configuración del nivel medio de la escala de tiempo de la vista. |
| [getNonWorkingTimeColor()](#getNonWorkingTimeColor--) | Obtiene el color del tiempo no laborable. |
| [getProgressLines()](#getProgressLines--) | Obtiene las líneas de progreso para la vista de diagrama de Gantt. |
| [getRollUpGanttBars()](#getRollUpGanttBars--) | Obtiene un valor que indica si las barras en el diagrama de Gantt deben consolidarse. |
| [getShowBarSplits()](#getShowBarSplits--) | Obtiene un valor que indica si se deben mostrar las divisiones de tareas en el diagrama de Gantt. |
| [getShowDrawings()](#getShowDrawings--) | Obtiene un valor que indica si se deben mostrar los dibujos en el diagrama de Gantt. |
| [getTableTextStyles()](#getTableTextStyles--) | Obtiene una lista de estilos de texto de tabla de la vista de diagrama de Gantt. |
| [getTextStyles()](#getTextStyles--) | Obtiene una lista de [TextStyle](../../com.aspose.tasks/textstyle) de la vista de diagrama de Gantt. |
| [getTimescaleSizePercentage()](#getTimescaleSizePercentage--) | \{@inheritDoc\} |
| [getTopTimescaleTier()](#getTopTimescaleTier--) | Obtiene la configuración del nivel superior de la escala de tiempo de la vista. |
| [setBarRounding(boolean value)](#setBarRounding-boolean-) | Establece un valor que indica si las barras se redondean al día más cercano. |
| [setBarSize(int value)](#setBarSize-int-) | Establece la altura, en puntos, de las barras de Gantt en el diagrama de Gantt. |
| [setBottomTimescaleTier(TimescaleTier value)](#setBottomTimescaleTier-com.aspose.tasks.TimescaleTier-) | Establece la configuración del nivel inferior de la escala de tiempo de la vista. |
| [setGridlines(List&lt;Gridlines&gt; value)](#setGridlines-java.util.List-com.aspose.tasks.Gridlines--) | Establece una lista de `Gridlines`([getGridlines()](../../com.aspose/tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose/tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) de la vista del diagrama de Gantt. |
| [setHideRollupBarsWhenSummaryExpanded(boolean value)](#setHideRollupBarsWhenSummaryExpanded-boolean-) | Establece un valor que indica si las barras de consolidación se ocultarán al expandir la tarea resumida. |
| [setMiddleTimescaleTier(TimescaleTier value)](#setMiddleTimescaleTier-com.aspose.tasks.TimescaleTier-) | Establece la configuración del nivel medio de escala de tiempo de la vista. |
| [setNonWorkingTimeColor(Color value)](#setNonWorkingTimeColor-java.awt.Color-) | Establece el color del tiempo no laborable. |
| [setProgressLines(ProgressLines value)](#setProgressLines-com.aspose.tasks.ProgressLines-) | Establece las líneas de progreso para la vista del diagrama de Gantt. |
| [setRollUpGanttBars(boolean value)](#setRollUpGanttBars-boolean-) | Establece un valor que indica si las barras en el diagrama de Gantt deben consolidarse. |
| [setShowBarSplits(boolean value)](#setShowBarSplits-boolean-) | Establece un valor que indica si las divisiones de tareas en el diagrama de Gantt deben mostrarse. |
| [setShowDrawings(boolean value)](#setShowDrawings-boolean-) | Establece un valor que indica si los dibujos en el diagrama de Gantt deben mostrarse. |
| [setTextStyles(List&lt;TextStyle&gt; value)](#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--) | Establece una lista de [TextStyle](../../com.aspose.tasks/textstyle) de la vista del diagrama de Gantt. |
| [setTimescaleSizePercentage(int value)](#setTimescaleSizePercentage-int-) | \{@inheritDoc\} |
| [setTopTimescaleTier(TimescaleTier value)](#setTopTimescaleTier-com.aspose.tasks.TimescaleTier-) | Establece la configuración del nivel superior de escala de tiempo de la vista. |
### GanttChartView() {#GanttChartView--}
```
public GanttChartView()
```


Inicializa una nueva instancia de la clase [GanttChartView](../../com.aspose.tasks/ganttchartview).

### getAutoFilters() {#getAutoFilters--}
```
public final FilterCollection getAutoFilters()
```


Obtiene una lista de filtros automáticos de una vista de diagrama de Gantt.

**Returns:**
[FilterCollection](../../com.aspose.tasks/filtercollection) - a list of auto filters of a Gantt Chart view.
### getBarRounding() {#getBarRounding--}
```
public final boolean getBarRounding()
```


Obtiene un valor que indica si las barras se redondean al día más cercano. El valor predeterminado es True.

**Returns:**
boolean - un valor que indica si las barras se redondean al día más cercano.
### getBarSize() {#getBarSize--}
```
public final int getBarSize()
```


Obtiene la altura, en puntos, de las barras de Gantt en el diagrama de Gantt.

**Returns:**
int - la altura, en puntos, de las barras de Gantt en el diagrama de Gantt.
### getBarStyles() {#getBarStyles--}
```
public final List<GanttBarStyle> getBarStyles()
```


Obtiene una lista de estilos de barra padre (comunes) de la vista del diagrama de Gantt. [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle).

**Returns:**
java.util.List&lt;com.aspose.tasks.GanttBarStyle&gt; - una lista de estilos de barra padre (comunes) de la vista del diagrama de Gantt.
### getBottomTimescaleTier() {#getBottomTimescaleTier--}
```
public final TimescaleTier getBottomTimescaleTier()
```


Obtiene la configuración del nivel inferior de escala de tiempo de la vista. [TimescaleTier](../../com.aspose.tasks/timescaletier)

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's bottom timescale tier.
### getCustomBarStyles() {#getCustomBarStyles--}
```
public final List<GanttBarStyle> getCustomBarStyles()
```


Obtiene una lista de estilos de barra personalizados específicos de tareas de la vista del diagrama de Gantt. [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle).

**Returns:**
java.util.List&lt;com.aspose.tasks.GanttBarStyle&gt; - una lista de estilos de barra personalizados específicos de tareas de la vista del diagrama de Gantt.
### getGridlines() {#getGridlines--}
```
public final List<Gridlines> getGridlines()
```


Obtiene una lista de `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) de la vista de diagrama de Gantt.

**Returns:**
java.util.List&lt;com.aspose.tasks.Gridlines&gt; - una lista de `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) de la vista del diagrama de Gantt.
### getHideRollupBarsWhenSummaryExpanded() {#getHideRollupBarsWhenSummaryExpanded--}
```
public final boolean getHideRollupBarsWhenSummaryExpanded()
```


Obtiene un valor que indica si las barras de consolidación se ocultarán al expandir la tarea resumen.

**Returns:**
boolean - un valor que indica si las barras de consolidación se ocultarán al expandir la tarea resumida.
### getMiddleTimescaleTier() {#getMiddleTimescaleTier--}
```
public final TimescaleTier getMiddleTimescaleTier()
```


Obtiene la configuración del nivel medio de escala de tiempo de la vista. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's middle timescale tier.
### getNonWorkingTimeColor() {#getNonWorkingTimeColor--}
```
public final Color getNonWorkingTimeColor()
```


Obtiene el color del tiempo no laborable.

**Returns:**
java.awt.Color - color del tiempo no laborable.
### getProgressLines() {#getProgressLines--}
```
public final ProgressLines getProgressLines()
```


Obtiene las líneas de progreso para la vista del diagrama de Gantt. `ProgressLines`([getProgressLines()](../../com.aspose.tasks/ganttchartview\#getProgressLines--)/[setProgressLines(ProgressLines)](../../com.aspose.tasks/ganttchartview\#setProgressLines-ProgressLines-)).

**Returns:**
[ProgressLines](../../com.aspose.tasks/progresslines) - progress lines for the Gantt Chart view.
### getRollUpGanttBars() {#getRollUpGanttBars--}
```
public final boolean getRollUpGanttBars()
```


Obtiene un valor que indica si las barras en el diagrama de Gantt deben consolidarse.

**Returns:**
boolean - un valor que indica si las barras en el diagrama de Gantt deben consolidarse.
### getShowBarSplits() {#getShowBarSplits--}
```
public final boolean getShowBarSplits()
```


Obtiene un valor que indica si se deben mostrar las divisiones de tareas en el diagrama de Gantt.

**Returns:**
boolean - un valor que indica si las divisiones de tareas en el diagrama de Gantt deben mostrarse.
### getShowDrawings() {#getShowDrawings--}
```
public final boolean getShowDrawings()
```


Obtiene un valor que indica si se deben mostrar los dibujos en el diagrama de Gantt.

**Returns:**
boolean - un valor que indica si los dibujos en el diagrama de Gantt deben mostrarse.
### getTableTextStyles() {#getTableTextStyles--}
```
public final List<TableTextStyle> getTableTextStyles()
```


Obtiene una lista de estilos de texto de tabla de la vista del diagrama de Gantt. [TableTextStyle](../../com.aspose.tasks/tabletextstyle).

**Returns:**
java.util.List&lt;com.aspose.tasks.TableTextStyle&gt; - una lista de estilos de texto de tabla de la vista del diagrama de Gantt.
### getTextStyles() {#getTextStyles--}
```
public final List<TextStyle> getTextStyles()
```


Obtiene una lista de [TextStyle](../../com.aspose.tasks/textstyle) de la vista de diagrama de Gantt.

**Returns:**
java.util.List&lt;com.aspose.tasks.TextStyle&gt; - una lista de [TextStyle](../../com.aspose.tasks/textstyle) de la vista del diagrama de Gantt.
### getTimescaleSizePercentage() {#getTimescaleSizePercentage--}
```
public final int getTimescaleSizePercentage()
```


Obtiene un porcentaje para reducir o ampliar el espaciado entre unidades en el nivel de escala de tiempo.

**Returns:**
int - \{@inheritDoc\}
### getTopTimescaleTier() {#getTopTimescaleTier--}
```
public final TimescaleTier getTopTimescaleTier()
```


Obtiene la configuración del nivel superior de escala de tiempo de la vista. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's top timescale tier.
### setBarRounding(boolean value) {#setBarRounding-boolean-}
```
public final void setBarRounding(boolean value)
```


Establece un valor que indica si las barras se redondean al día más cercano. El valor predeterminado es True.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si las barras se redondean al día más cercano. |

### setBarSize(int value) {#setBarSize-int-}
```
public final void setBarSize(int value)
```


Establece la altura, en puntos, de las barras de Gantt en el diagrama de Gantt.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | la altura, en puntos, de las barras Gantt en el diagrama de Gantt. |

### setBottomTimescaleTier(TimescaleTier value) {#setBottomTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setBottomTimescaleTier(TimescaleTier value)
```


Establece la configuración del nivel inferior de escala de tiempo de la vista. [TimescaleTier](../../com.aspose.tasks/timescaletier)

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | configuración del nivel inferior de escala de tiempo de la vista. |

### setGridlines(List&lt;Gridlines&gt; value) {#setGridlines-java.util.List-com.aspose.tasks.Gridlines--}
```
public final void setGridlines(List<Gridlines> value)
```


Establece una lista de `Gridlines`([getGridlines()](../../com.aspose/tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose/tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) de la vista del diagrama de Gantt.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.Gridlines&gt; | una lista de `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) de la vista del diagrama de Gantt. |

### setHideRollupBarsWhenSummaryExpanded(boolean value) {#setHideRollupBarsWhenSummaryExpanded-boolean-}
```
public final void setHideRollupBarsWhenSummaryExpanded(boolean value)
```


Establece un valor que indica si las barras de consolidación se ocultarán al expandir la tarea resumida.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si las barras de consolidación se ocultarán al expandir la tarea resumen. |

### setMiddleTimescaleTier(TimescaleTier value) {#setMiddleTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setMiddleTimescaleTier(TimescaleTier value)
```


Establece la configuración del nivel medio de escala de tiempo de la vista. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | configuración del nivel medio de escala de tiempo de la vista. |

### setNonWorkingTimeColor(Color value) {#setNonWorkingTimeColor-java.awt.Color-}
```
public final void setNonWorkingTimeColor(Color value)
```


Establece el color del tiempo no laborable.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.awt.Color | color de tiempo no laborable. |

### setProgressLines(ProgressLines value) {#setProgressLines-com.aspose.tasks.ProgressLines-}
```
public final void setProgressLines(ProgressLines value)
```


Establece líneas de progreso para la vista del diagrama de Gantt. `ProgressLines`([getProgressLines()](../../com.aspose.tasks/ganttchartview\#getProgressLines--)/[setProgressLines(ProgressLines)](../../com.aspose.tasks/ganttchartview\#setProgressLines-ProgressLines-)).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [ProgressLines](../../com.aspose.tasks/progresslines) | líneas de progreso para la vista del diagrama de Gantt. |

### setRollUpGanttBars(boolean value) {#setRollUpGanttBars-boolean-}
```
public final void setRollUpGanttBars(boolean value)
```


Establece un valor que indica si las barras en el diagrama de Gantt deben consolidarse.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si las barras en el diagrama de Gantt deben consolidarse. |

### setShowBarSplits(boolean value) {#setShowBarSplits-boolean-}
```
public final void setShowBarSplits(boolean value)
```


Establece un valor que indica si las divisiones de tareas en el diagrama de Gantt deben mostrarse.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si las divisiones de tareas en el diagrama de Gantt deben mostrarse. |

### setShowDrawings(boolean value) {#setShowDrawings-boolean-}
```
public final void setShowDrawings(boolean value)
```


Establece un valor que indica si los dibujos en el diagrama de Gantt deben mostrarse.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | un valor que indica si los dibujos en el diagrama de Gantt deben mostrarse. |

### setTextStyles(List&lt;TextStyle&gt; value) {#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--}
```
public final void setTextStyles(List<TextStyle> value)
```


Establece una lista de [TextStyle](../../com.aspose.tasks/textstyle) de la vista del diagrama de Gantt.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.TextStyle&gt; | una lista de [TextStyle](../../com.aspose.tasks/textstyle) de la vista del diagrama de Gantt. |

### setTimescaleSizePercentage(int value) {#setTimescaleSizePercentage-int-}
```
public final void setTimescaleSizePercentage(int value)
```


Establece un porcentaje para reducir o ampliar el espaciado entre unidades en el nivel de escala de tiempo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | \{@inheritDoc\} |

### setTopTimescaleTier(TimescaleTier value) {#setTopTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setTopTimescaleTier(TimescaleTier value)
```


Establece la configuración del nivel superior de escala de tiempo de la vista. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | configuración del nivel superior de escala de tiempo de la vista. |

