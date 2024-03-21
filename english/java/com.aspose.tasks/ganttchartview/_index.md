---
title: GanttChartView
second_title: Aspose.Tasks for Java API Reference
description: Represents a GanttChart view.
type: docs
weight: 112
url: /java/com.aspose.tasks/ganttchartview/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.View](../../com.aspose.tasks/view)

**All Implemented Interfaces:**
com.aspose.tasks.ITimescaledView
```
public class GanttChartView extends View implements ITimescaledView
```

Represents a GanttChart view.
## Constructors

| Constructor | Description |
| --- | --- |
| [GanttChartView()](#GanttChartView--) | Initializes a new instance of the [GanttChartView](../../com.aspose.tasks/ganttchartview) class. |
## Methods

| Method | Description |
| --- | --- |
| [getAutoFilters()](#getAutoFilters--) | Gets a list of auto filters of a Gantt Chart view. |
| [getBarRounding()](#getBarRounding--) | Gets a value indicating whether the bars round to the nearest day. |
| [getBarSize()](#getBarSize--) | Gets the height, in points, of the Gantt bars in the Gantt Chart. |
| [getBarStyles()](#getBarStyles--) | Gets a list of parent (common) bar styles of the Gantt Chart view. |
| [getBottomTimescaleTier()](#getBottomTimescaleTier--) | Gets settings of view's bottom timescale tier. |
| [getCustomBarStyles()](#getCustomBarStyles--) | Gets a list of custom task-specific bar styles of the Gantt Chart view. |
| [getGridlines()](#getGridlines--) | Gets a list of `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) of the Gantt Chart view. |
| [getHideRollupBarsWhenSummaryExpanded()](#getHideRollupBarsWhenSummaryExpanded--) | Gets a value indicating whether rollup bars will be hidden when expanding summary task. |
| [getMiddleTimescaleTier()](#getMiddleTimescaleTier--) | Gets settings of view's middle timescale tier. |
| [getNonWorkingTimeColor()](#getNonWorkingTimeColor--) | Gets non-working time color. |
| [getProgressLines()](#getProgressLines--) | Gets progress lines for the Gantt Chart view. |
| [getRollUpGanttBars()](#getRollUpGanttBars--) | Gets a value indicating whether bars on the Gantt Chart must be rolled up. |
| [getShowBarSplits()](#getShowBarSplits--) | Gets a value indicating whether task splits on the Gantt Chart must be shown. |
| [getShowDrawings()](#getShowDrawings--) | Gets a value indicating whether drawings on the Gantt Chart must be shown. |
| [getTableTextStyles()](#getTableTextStyles--) | Gets a list of table text styles of the Gantt Chart view. |
| [getTextStyles()](#getTextStyles--) | Gets a list of [TextStyle](../../com.aspose.tasks/textstyle) of the Gantt Chart view. |
| [getTimescaleSizePercentage()](#getTimescaleSizePercentage--) | \{@inheritDoc\} |
| [getTopTimescaleTier()](#getTopTimescaleTier--) | Gets settings of view's top timescale tier. |
| [setBarRounding(boolean value)](#setBarRounding-boolean-) | Sets a value indicating whether the bars round to the nearest day. |
| [setBarSize(int value)](#setBarSize-int-) | Sets the height, in points, of the Gantt bars in the Gantt Chart. |
| [setBottomTimescaleTier(TimescaleTier value)](#setBottomTimescaleTier-com.aspose.tasks.TimescaleTier-) | Sets settings of view's bottom timescale tier. |
| [setGridlines(List&lt;Gridlines&gt; value)](#setGridlines-java.util.List-com.aspose.tasks.Gridlines--) | Sets a list of `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) of the Gantt Chart view. |
| [setHideRollupBarsWhenSummaryExpanded(boolean value)](#setHideRollupBarsWhenSummaryExpanded-boolean-) | Sets a value indicating whether rollup bars will be hidden when expanding summary task. |
| [setMiddleTimescaleTier(TimescaleTier value)](#setMiddleTimescaleTier-com.aspose.tasks.TimescaleTier-) | Sets settings of view's middle timescale tier. |
| [setNonWorkingTimeColor(Color value)](#setNonWorkingTimeColor-java.awt.Color-) | Sets non-working time color. |
| [setProgressLines(ProgressLines value)](#setProgressLines-com.aspose.tasks.ProgressLines-) | Sets progress lines for the Gantt Chart view. |
| [setRollUpGanttBars(boolean value)](#setRollUpGanttBars-boolean-) | Sets a value indicating whether bars on the Gantt Chart must be rolled up. |
| [setShowBarSplits(boolean value)](#setShowBarSplits-boolean-) | Sets a value indicating whether task splits on the Gantt Chart must be shown. |
| [setShowDrawings(boolean value)](#setShowDrawings-boolean-) | Sets a value indicating whether drawings on the Gantt Chart must be shown. |
| [setTextStyles(List&lt;TextStyle&gt; value)](#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--) | Sets a list of [TextStyle](../../com.aspose.tasks/textstyle) of the Gantt Chart view. |
| [setTimescaleSizePercentage(int value)](#setTimescaleSizePercentage-int-) | \{@inheritDoc\} |
| [setTopTimescaleTier(TimescaleTier value)](#setTopTimescaleTier-com.aspose.tasks.TimescaleTier-) | Sets settings of view's top timescale tier. |
### GanttChartView() {#GanttChartView--}
```
public GanttChartView()
```


Initializes a new instance of the [GanttChartView](../../com.aspose.tasks/ganttchartview) class.

### getAutoFilters() {#getAutoFilters--}
```
public final FilterCollection getAutoFilters()
```


Gets a list of auto filters of a Gantt Chart view.

**Returns:**
[FilterCollection](../../com.aspose.tasks/filtercollection) - a list of auto filters of a Gantt Chart view.
### getBarRounding() {#getBarRounding--}
```
public final boolean getBarRounding()
```


Gets a value indicating whether the bars round to the nearest day. The default value is True.

**Returns:**
boolean - a value indicating whether the bars round to the nearest day.
### getBarSize() {#getBarSize--}
```
public final int getBarSize()
```


Gets the height, in points, of the Gantt bars in the Gantt Chart.

**Returns:**
int - the height, in points, of the Gantt bars in the Gantt Chart.
### getBarStyles() {#getBarStyles--}
```
public final List<GanttBarStyle> getBarStyles()
```


Gets a list of parent (common) bar styles of the Gantt Chart view. [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle).

**Returns:**
java.util.List&lt;com.aspose.tasks.GanttBarStyle&gt; - a list of parent (common) bar styles of the Gantt Chart view.
### getBottomTimescaleTier() {#getBottomTimescaleTier--}
```
public final TimescaleTier getBottomTimescaleTier()
```


Gets settings of view's bottom timescale tier. [TimescaleTier](../../com.aspose.tasks/timescaletier)

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's bottom timescale tier.
### getCustomBarStyles() {#getCustomBarStyles--}
```
public final List<GanttBarStyle> getCustomBarStyles()
```


Gets a list of custom task-specific bar styles of the Gantt Chart view. [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle).

**Returns:**
java.util.List&lt;com.aspose.tasks.GanttBarStyle&gt; - a list of custom task-specific bar styles of the Gantt Chart view.
### getGridlines() {#getGridlines--}
```
public final List<Gridlines> getGridlines()
```


Gets a list of `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) of the Gantt Chart view.

**Returns:**
java.util.List&lt;com.aspose.tasks.Gridlines&gt; - a list of `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) of the Gantt Chart view.
### getHideRollupBarsWhenSummaryExpanded() {#getHideRollupBarsWhenSummaryExpanded--}
```
public final boolean getHideRollupBarsWhenSummaryExpanded()
```


Gets a value indicating whether rollup bars will be hidden when expanding summary task.

**Returns:**
boolean - a value indicating whether rollup bars will be hidden when expanding summary task.
### getMiddleTimescaleTier() {#getMiddleTimescaleTier--}
```
public final TimescaleTier getMiddleTimescaleTier()
```


Gets settings of view's middle timescale tier. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's middle timescale tier.
### getNonWorkingTimeColor() {#getNonWorkingTimeColor--}
```
public final Color getNonWorkingTimeColor()
```


Gets non-working time color.

**Returns:**
java.awt.Color - non-working time color.
### getProgressLines() {#getProgressLines--}
```
public final ProgressLines getProgressLines()
```


Gets progress lines for the Gantt Chart view. `ProgressLines`([getProgressLines()](../../com.aspose.tasks/ganttchartview\#getProgressLines--)/[setProgressLines(ProgressLines)](../../com.aspose.tasks/ganttchartview\#setProgressLines-ProgressLines-)).

**Returns:**
[ProgressLines](../../com.aspose.tasks/progresslines) - progress lines for the Gantt Chart view.
### getRollUpGanttBars() {#getRollUpGanttBars--}
```
public final boolean getRollUpGanttBars()
```


Gets a value indicating whether bars on the Gantt Chart must be rolled up.

**Returns:**
boolean - a value indicating whether bars on the Gantt Chart must be rolled up.
### getShowBarSplits() {#getShowBarSplits--}
```
public final boolean getShowBarSplits()
```


Gets a value indicating whether task splits on the Gantt Chart must be shown.

**Returns:**
boolean - a value indicating whether task splits on the Gantt Chart must be shown.
### getShowDrawings() {#getShowDrawings--}
```
public final boolean getShowDrawings()
```


Gets a value indicating whether drawings on the Gantt Chart must be shown.

**Returns:**
boolean - a value indicating whether drawings on the Gantt Chart must be shown.
### getTableTextStyles() {#getTableTextStyles--}
```
public final List<TableTextStyle> getTableTextStyles()
```


Gets a list of table text styles of the Gantt Chart view. [TableTextStyle](../../com.aspose.tasks/tabletextstyle).

**Returns:**
java.util.List&lt;com.aspose.tasks.TableTextStyle&gt; - a list of table text styles of the Gantt Chart view.
### getTextStyles() {#getTextStyles--}
```
public final List<TextStyle> getTextStyles()
```


Gets a list of [TextStyle](../../com.aspose.tasks/textstyle) of the Gantt Chart view.

**Returns:**
java.util.List&lt;com.aspose.tasks.TextStyle&gt; - a list of [TextStyle](../../com.aspose.tasks/textstyle) of the Gantt Chart view.
### getTimescaleSizePercentage() {#getTimescaleSizePercentage--}
```
public final int getTimescaleSizePercentage()
```


Gets a percentage to reduce or enlarge the spacing between units on the timescale tier.

**Returns:**
int - \{@inheritDoc\}
### getTopTimescaleTier() {#getTopTimescaleTier--}
```
public final TimescaleTier getTopTimescaleTier()
```


Gets settings of view's top timescale tier. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's top timescale tier.
### setBarRounding(boolean value) {#setBarRounding-boolean-}
```
public final void setBarRounding(boolean value)
```


Sets a value indicating whether the bars round to the nearest day. The default value is True.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether the bars round to the nearest day. |

### setBarSize(int value) {#setBarSize-int-}
```
public final void setBarSize(int value)
```


Sets the height, in points, of the Gantt bars in the Gantt Chart.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the height, in points, of the Gantt bars in the Gantt Chart. |

### setBottomTimescaleTier(TimescaleTier value) {#setBottomTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setBottomTimescaleTier(TimescaleTier value)
```


Sets settings of view's bottom timescale tier. [TimescaleTier](../../com.aspose.tasks/timescaletier)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | settings of view's bottom timescale tier. |

### setGridlines(List&lt;Gridlines&gt; value) {#setGridlines-java.util.List-com.aspose.tasks.Gridlines--}
```
public final void setGridlines(List<Gridlines> value)
```


Sets a list of `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) of the Gantt Chart view.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.Gridlines&gt; | a list of `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) of the Gantt Chart view. |

### setHideRollupBarsWhenSummaryExpanded(boolean value) {#setHideRollupBarsWhenSummaryExpanded-boolean-}
```
public final void setHideRollupBarsWhenSummaryExpanded(boolean value)
```


Sets a value indicating whether rollup bars will be hidden when expanding summary task.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether rollup bars will be hidden when expanding summary task. |

### setMiddleTimescaleTier(TimescaleTier value) {#setMiddleTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setMiddleTimescaleTier(TimescaleTier value)
```


Sets settings of view's middle timescale tier. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | settings of view's middle timescale tier. |

### setNonWorkingTimeColor(Color value) {#setNonWorkingTimeColor-java.awt.Color-}
```
public final void setNonWorkingTimeColor(Color value)
```


Sets non-working time color.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.awt.Color | non-working time color. |

### setProgressLines(ProgressLines value) {#setProgressLines-com.aspose.tasks.ProgressLines-}
```
public final void setProgressLines(ProgressLines value)
```


Sets progress lines for the Gantt Chart view. `ProgressLines`([getProgressLines()](../../com.aspose.tasks/ganttchartview\#getProgressLines--)/[setProgressLines(ProgressLines)](../../com.aspose.tasks/ganttchartview\#setProgressLines-ProgressLines-)).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ProgressLines](../../com.aspose.tasks/progresslines) | progress lines for the Gantt Chart view. |

### setRollUpGanttBars(boolean value) {#setRollUpGanttBars-boolean-}
```
public final void setRollUpGanttBars(boolean value)
```


Sets a value indicating whether bars on the Gantt Chart must be rolled up.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether bars on the Gantt Chart must be rolled up. |

### setShowBarSplits(boolean value) {#setShowBarSplits-boolean-}
```
public final void setShowBarSplits(boolean value)
```


Sets a value indicating whether task splits on the Gantt Chart must be shown.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether task splits on the Gantt Chart must be shown. |

### setShowDrawings(boolean value) {#setShowDrawings-boolean-}
```
public final void setShowDrawings(boolean value)
```


Sets a value indicating whether drawings on the Gantt Chart must be shown.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether drawings on the Gantt Chart must be shown. |

### setTextStyles(List&lt;TextStyle&gt; value) {#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--}
```
public final void setTextStyles(List<TextStyle> value)
```


Sets a list of [TextStyle](../../com.aspose.tasks/textstyle) of the Gantt Chart view.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.TextStyle&gt; | a list of [TextStyle](../../com.aspose.tasks/textstyle) of the Gantt Chart view. |

### setTimescaleSizePercentage(int value) {#setTimescaleSizePercentage-int-}
```
public final void setTimescaleSizePercentage(int value)
```


Sets a percentage to reduce or enlarge the spacing between units on the timescale tier.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | \{@inheritDoc\} |

### setTopTimescaleTier(TimescaleTier value) {#setTopTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setTopTimescaleTier(TimescaleTier value)
```


Sets settings of view's top timescale tier. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | settings of view's top timescale tier. |

