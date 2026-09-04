---
title: "GanttChartView"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示甘特图视图。"
type: docs
weight: 112
url: /zh/java/com.aspose.tasks/ganttchartview/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.View](../../com.aspose.tasks/view)

**All Implemented Interfaces:**
com.aspose.tasks.ITimescaledView
```
public class GanttChartView extends View implements ITimescaledView
```

表示甘特图视图。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [GanttChartView()](#GanttChartView--) | 初始化 [GanttChartView](../../com.aspose.tasks/ganttchartview) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [getAutoFilters()](#getAutoFilters--) | 获取甘特图视图的自动筛选器列表。 |
| [getBarRounding()](#getBarRounding--) | 获取一个值，指示条形是否四舍五入到最近的一天。 |
| [getBarSize()](#getBarSize--) | 获取甘特图中甘特条的高度（单位：点）。 |
| [getBarStyles()](#getBarStyles--) | 获取甘特图视图的父（通用）条样式列表。 |
| [getBottomTimescaleTier()](#getBottomTimescaleTier--) | 获取视图底部时间刻度层的设置。 |
| [getCustomBarStyles()](#getCustomBarStyles--) | 获取甘特图视图的自定义任务特定条样式列表。 |
| [getGridlines()](#getGridlines--) | 获取甘特图视图的 `Gridlines` 列表([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--))。 |
| [getHideRollupBarsWhenSummaryExpanded()](#getHideRollupBarsWhenSummaryExpanded--) | 获取一个值，指示在展开汇总任务时是否隐藏汇总条。 |
| [getMiddleTimescaleTier()](#getMiddleTimescaleTier--) | 获取视图中部时间刻度层的设置。 |
| [getNonWorkingTimeColor()](#getNonWorkingTimeColor--) | 获取非工作时间颜色。 |
| [getProgressLines()](#getProgressLines--) | 获取甘特图视图的进度线。 |
| [getRollUpGanttBars()](#getRollUpGanttBars--) | 获取一个值，指示甘特图上的条是否必须汇总。 |
| [getShowBarSplits()](#getShowBarSplits--) | 获取一个值，指示甘特图上的任务拆分是否必须显示。 |
| [getShowDrawings()](#getShowDrawings--) | 获取一个值，指示甘特图上的绘图是否必须显示。 |
| [getTableTextStyles()](#getTableTextStyles--) | 获取甘特图视图的表格文本样式列表。 |
| [getTextStyles()](#getTextStyles--) | 获取甘特图视图的 [TextStyle](../../com.aspose.tasks/textstyle) 列表。 |
| [getTimescaleSizePercentage()](#getTimescaleSizePercentage--) | \{@inheritDoc\} |
| [getTopTimescaleTier()](#getTopTimescaleTier--) | 获取视图顶部时间刻度层的设置。 |
| [setBarRounding(boolean value)](#setBarRounding-boolean-) | 设置一个值，指示条形是否四舍五入到最近的一天。 |
| [setBarSize(int value)](#setBarSize-int-) | 设置甘特图中甘特条的高度（单位：点）。 |
| [setBottomTimescaleTier(TimescaleTier value)](#setBottomTimescaleTier-com.aspose.tasks.TimescaleTier-) | 设置视图底部时间刻度层的设置。 |
| [setGridlines(List&lt;Gridlines&gt; value)](#setGridlines-java.util.List-com.aspose.tasks.Gridlines--) | 设置甘特图视图的 `Gridlines` 列表([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--))。 |
| [setHideRollupBarsWhenSummaryExpanded(boolean value)](#setHideRollupBarsWhenSummaryExpanded-boolean-) | 设置一个值，指示在展开汇总任务时是否隐藏汇总条。 |
| [setMiddleTimescaleTier(TimescaleTier value)](#setMiddleTimescaleTier-com.aspose.tasks.TimescaleTier-) | 设置视图的中间时间刻度层的设置。 |
| [setNonWorkingTimeColor(Color value)](#setNonWorkingTimeColor-java.awt.Color-) | 设置非工作时间颜色。 |
| [setProgressLines(ProgressLines value)](#setProgressLines-com.aspose.tasks.ProgressLines-) | 设置甘特图视图的进度线。 |
| [setRollUpGanttBars(boolean value)](#setRollUpGanttBars-boolean-) | 设置一个值，指示甘特图上的条是否必须汇总。 |
| [setShowBarSplits(boolean value)](#setShowBarSplits-boolean-) | 设置一个值，指示甘特图上的任务拆分是否必须显示。 |
| [setShowDrawings(boolean value)](#setShowDrawings-boolean-) | 设置一个值，指示甘特图上的绘图是否必须显示。 |
| [setTextStyles(List&lt;TextStyle&gt; value)](#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--) | 设置甘特图视图的 [TextStyle](../../com.aspose.tasks/textstyle) 列表。 |
| [setTimescaleSizePercentage(int value)](#setTimescaleSizePercentage-int-) | \{@inheritDoc\} |
| [setTopTimescaleTier(TimescaleTier value)](#setTopTimescaleTier-com.aspose.tasks.TimescaleTier-) | 设置视图的顶部时间刻度层的设置。 |
### GanttChartView() {#GanttChartView--}
```
public GanttChartView()
```


初始化 [GanttChartView](../../com.aspose.tasks/ganttchartview) 类的新实例。

### getAutoFilters() {#getAutoFilters--}
```
public final FilterCollection getAutoFilters()
```


获取甘特图视图的自动筛选器列表。

**Returns:**
[FilterCollection](../../com.aspose.tasks/filtercollection) - a list of auto filters of a Gantt Chart view.
### getBarRounding() {#getBarRounding--}
```
public final boolean getBarRounding()
```


获取一个值，指示条形是否四舍五入到最近的一天。默认值为 True。

**Returns:**
boolean - 一个指示条形是否四舍五入到最近一天的值。
### getBarSize() {#getBarSize--}
```
public final int getBarSize()
```


获取甘特图中甘特条的高度（单位：点）。

**Returns:**
int - Gantt 图表中甘特条的高度（单位为点）。
### getBarStyles() {#getBarStyles--}
```
public final List<GanttBarStyle> getBarStyles()
```


获取 Gantt 图表视图的父（通用）条形样式列表。 [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle)。

**Returns:**
java.util.List&lt;com.aspose.tasks.GanttBarStyle&gt; - Gantt 图表视图的父（通用）条形样式列表。
### getBottomTimescaleTier() {#getBottomTimescaleTier--}
```
public final TimescaleTier getBottomTimescaleTier()
```


获取视图的底部时间刻度层的设置。 [TimescaleTier](../../com.aspose.tasks/timescaletier)

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's bottom timescale tier.
### getCustomBarStyles() {#getCustomBarStyles--}
```
public final List<GanttBarStyle> getCustomBarStyles()
```


获取 Gantt 图表视图的自定义任务特定条形样式列表。 [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle)。

**Returns:**
java.util.List&lt;com.aspose.tasks.GanttBarStyle&gt; - Gantt 图表视图的自定义任务特定条形样式列表。
### getGridlines() {#getGridlines--}
```
public final List<Gridlines> getGridlines()
```


获取甘特图视图的 `Gridlines` 列表([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--))。

**Returns:**
java.util.List&lt;com.aspose.tasks.Gridlines&gt; - Gantt 图表视图的 `Gridlines` 列表（[getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)）。
### getHideRollupBarsWhenSummaryExpanded() {#getHideRollupBarsWhenSummaryExpanded--}
```
public final boolean getHideRollupBarsWhenSummaryExpanded()
```


获取一个值，指示在展开汇总任务时是否隐藏汇总条。

**Returns:**
boolean - 一个指示在展开汇总任务时是否隐藏汇总条形的值。
### getMiddleTimescaleTier() {#getMiddleTimescaleTier--}
```
public final TimescaleTier getMiddleTimescaleTier()
```


获取视图的中间时间刻度层的设置。 [TimescaleTier](../../com.aspose.tasks/timescaletier)。

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's middle timescale tier.
### getNonWorkingTimeColor() {#getNonWorkingTimeColor--}
```
public final Color getNonWorkingTimeColor()
```


获取非工作时间颜色。

**Returns:**
java.awt.Color - 非工作时间颜色。
### getProgressLines() {#getProgressLines--}
```
public final ProgressLines getProgressLines()
```


获取 Gantt 图表视图的进度线。 `ProgressLines`（[getProgressLines()](../../com.aspose.tasks/ganttchartview\#getProgressLines--)/[setProgressLines(ProgressLines)](../../com.aspose.tasks/ganttchartview\#setProgressLines-ProgressLines-)）。

**Returns:**
[ProgressLines](../../com.aspose.tasks/progresslines) - progress lines for the Gantt Chart view.
### getRollUpGanttBars() {#getRollUpGanttBars--}
```
public final boolean getRollUpGanttBars()
```


获取一个值，指示甘特图上的条是否必须汇总。

**Returns:**
boolean - 一个指示 Gantt 图表上的条形是否必须汇总的值。
### getShowBarSplits() {#getShowBarSplits--}
```
public final boolean getShowBarSplits()
```


获取一个值，指示甘特图上的任务拆分是否必须显示。

**Returns:**
boolean - 一个指示是否必须显示 Gantt 图表上的任务拆分的值。
### getShowDrawings() {#getShowDrawings--}
```
public final boolean getShowDrawings()
```


获取一个值，指示甘特图上的绘图是否必须显示。

**Returns:**
boolean - 一个指示是否必须显示 Gantt 图表上的绘图的值。
### getTableTextStyles() {#getTableTextStyles--}
```
public final List<TableTextStyle> getTableTextStyles()
```


获取 Gantt 图表视图的表格文本样式列表。 [TableTextStyle](../../com.aspose.tasks/tabletextstyle)。

**Returns:**
java.util.List&lt;com.aspose.tasks.TableTextStyle&gt; - Gantt 图表视图的表格文本样式列表。
### getTextStyles() {#getTextStyles--}
```
public final List<TextStyle> getTextStyles()
```


获取甘特图视图的 [TextStyle](../../com.aspose.tasks/textstyle) 列表。

**Returns:**
java.util.List&lt;com.aspose.tasks.TextStyle&gt; - Gantt 图表视图的 [TextStyle](../../com.aspose.tasks/textstyle) 列表。
### getTimescaleSizePercentage() {#getTimescaleSizePercentage--}
```
public final int getTimescaleSizePercentage()
```


获取用于在时间刻度层上缩小或放大单位之间间距的百分比。

**Returns:**
int - \{@inheritDoc\}
### getTopTimescaleTier() {#getTopTimescaleTier--}
```
public final TimescaleTier getTopTimescaleTier()
```


获取视图的顶部时间刻度层的设置。 [TimescaleTier](../../com.aspose.tasks/timescaletier)。

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's top timescale tier.
### setBarRounding(boolean value) {#setBarRounding-boolean-}
```
public final void setBarRounding(boolean value)
```


设置一个指示条形是否四舍五入到最近一天的值。默认值为 True。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 一个指示条形是否四舍五入到最近一天的值。 |

### setBarSize(int value) {#setBarSize-int-}
```
public final void setBarSize(int value)
```


设置甘特图中甘特条的高度（单位：点）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | Gantt 图表中甘特条的高度（单位为点）。 |

### setBottomTimescaleTier(TimescaleTier value) {#setBottomTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setBottomTimescaleTier(TimescaleTier value)
```


设置视图的底部时间刻度层的设置。 [TimescaleTier](../../com.aspose.tasks/timescaletier)

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | 视图的底部时间刻度层的设置。 |

### setGridlines(List&lt;Gridlines&gt; value) {#setGridlines-java.util.List-com.aspose.tasks.Gridlines--}
```
public final void setGridlines(List<Gridlines> value)
```


设置甘特图视图的 `Gridlines` 列表([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--))。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.Gridlines&gt; | Gantt 图表视图的 `Gridlines` 列表（[getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)）。 |

### setHideRollupBarsWhenSummaryExpanded(boolean value) {#setHideRollupBarsWhenSummaryExpanded-boolean-}
```
public final void setHideRollupBarsWhenSummaryExpanded(boolean value)
```


设置一个值，指示在展开汇总任务时是否隐藏汇总条。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 一个指示在展开汇总任务时是否隐藏汇总条形的值。 |

### setMiddleTimescaleTier(TimescaleTier value) {#setMiddleTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setMiddleTimescaleTier(TimescaleTier value)
```


设置视图的中间时间刻度层的设置。 [TimescaleTier](../../com.aspose.tasks/timescaletier)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | 视图的中间时间刻度层的设置。 |

### setNonWorkingTimeColor(Color value) {#setNonWorkingTimeColor-java.awt.Color-}
```
public final void setNonWorkingTimeColor(Color value)
```


设置非工作时间颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.awt.Color | 非工作时间颜色。 |

### setProgressLines(ProgressLines value) {#setProgressLines-com.aspose.tasks.ProgressLines-}
```
public final void setProgressLines(ProgressLines value)
```


设置 Gantt 图表视图的进度线。 `ProgressLines`（[getProgressLines()](../../com.aspose.tasks/ganttchartview\#getProgressLines--)/[setProgressLines(ProgressLines)](../../com.aspose.tasks/ganttchartview\#setProgressLines-ProgressLines-)）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [ProgressLines](../../com.aspose.tasks/progresslines) | Gantt 图表视图的进度线。 |

### setRollUpGanttBars(boolean value) {#setRollUpGanttBars-boolean-}
```
public final void setRollUpGanttBars(boolean value)
```


设置一个值，指示甘特图上的条是否必须汇总。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 一个指示 Gantt 图表上的条形是否必须汇总的值。 |

### setShowBarSplits(boolean value) {#setShowBarSplits-boolean-}
```
public final void setShowBarSplits(boolean value)
```


设置一个值，指示甘特图上的任务拆分是否必须显示。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示是否必须在甘特图上显示任务拆分的值。 |

### setShowDrawings(boolean value) {#setShowDrawings-boolean-}
```
public final void setShowDrawings(boolean value)
```


设置一个值，指示甘特图上的绘图是否必须显示。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示是否必须在甘特图上显示绘图的值。 |

### setTextStyles(List&lt;TextStyle&gt; value) {#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--}
```
public final void setTextStyles(List<TextStyle> value)
```


设置甘特图视图的 [TextStyle](../../com.aspose.tasks/textstyle) 列表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.TextStyle&gt; | 甘特图视图的 [TextStyle](../../com.aspose.tasks/textstyle) 列表。 |

### setTimescaleSizePercentage(int value) {#setTimescaleSizePercentage-int-}
```
public final void setTimescaleSizePercentage(int value)
```


设置用于在时间刻度层上缩小或放大单位之间间距的百分比。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | \{@inheritDoc\} |

### setTopTimescaleTier(TimescaleTier value) {#setTopTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setTopTimescaleTier(TimescaleTier value)
```


设置视图的顶部时间刻度层的设置。 [TimescaleTier](../../com.aspose.tasks/timescaletier)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | 视图的顶部时间刻度层的设置。 |

