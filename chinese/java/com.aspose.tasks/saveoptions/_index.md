---
title: "SaveOptions"
second_title: "Aspose.Tasks for Java API 参考"
description: "这是一个抽象基类，供允许用户在将项目保存为特定格式时指定附加选项的类使用。"
type: docs
weight: 274
url: /zh/java/com.aspose.tasks/saveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public abstract class SaveOptions extends SimpleSaveOptions
```

这是一个抽象基类，供允许用户在将项目保存为特定格式时指定附加选项的类使用。

--------------------

任意从 SaveOptions 类派生的类的实例会传递给流 Save 或字符串 Save 重载，以便用户在保存文档时定义自定义选项。
## 方法

| 方法 | 描述 |
| --- | --- |
| [getBarStyles()](#getBarStyles--) | 获取在项目视图中出现的 [BarStyle](../../com.aspose.tasks/barstyle) 类实例列表。 |
| [getCustomPageSize()](#getCustomPageSize--) | 获取自定义页面尺寸（单位：点，1 点 = 1/72 英寸）。 |
| [getDrawNonWorkingTime()](#getDrawNonWorkingTime--) | 获取一个值，指示是否应绘制非工作时间（默认值为 TRUE）。 |
| [getEndDate()](#getEndDate--) | 获取用于结束渲染的日期。 |
| [getFitContent()](#getFitContent--) | 获取一个值，指示是否应增加行高以适应其内容。 |
| [getGridlines()](#getGridlines--) | 获取在项目视图中出现的 [Gridline](../../com.aspose.tasks/gridline) 列表。 |
| [getLegendDrawingOptions()](#getLegendDrawingOptions--) | 获取一个值，用于定义图例的渲染方式。 |
| [getLegendItems()](#getLegendItems--) | 获取一个 PageLegendItem 数组，用于定义哪些条形应在页面图例中渲染。 |
| [getMarkCriticalTasks()](#getMarkCriticalTasks--) | 获取一个值，指示是否应以红色显示关键任务（默认值为 FALSE）。 |
| [getNonWorkingTimeColor()](#getNonWorkingTimeColor--) | 获取非工作时间的颜色。 |
| [getPageCount()](#getPageCount--) | 获取项目的页数。 |
| [getPageSize()](#getPageSize--) | 获取要渲染的页面大小（默认值为 PageSize.A4）。 |
| [getPresentationFormat()](#getPresentationFormat--) | 获取文档将被保存的 `PresentationFormat`（[getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-))。 |
| [getRenderToSinglePage()](#getRenderToSinglePage--) | 获取一个值，指示在以图形格式保存项目时是否应将项目渲染为单页。 |
| [getRollUpGanttBars()](#getRollUpGanttBars--) | 获取一个值，指示是否应标记汇总任务栏上的子任务。 |
| [getStartDate()](#getStartDate--) | 获取渲染的起始日期。 |
| [getTaskLinkDrawingCallback()](#getTaskLinkDrawingCallback--) | 获取一个回调，可用于自定义任务链接渲染的某些方面。 |
| [getTextStyles()](#getTextStyles--) | 获取在项目视图渲染期间应用的文本样式列表。 |
| [getTimescale()](#getTimescale--) | 获取用于控制在项目保存为图形格式时时间刻度（如果存在）如何渲染的 `Timescale`（[getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) 值。 |
| [getTimescaleFitBehavior()](#getTimescaleFitBehavior--) | 获取一种行为，定义如何将时间刻度的右端与页面末端对齐。 |
| [getUseGradientBrush()](#getUseGradientBrush--) | 获取一个值，指示在渲染甘特图时是否应使用渐变画笔。 |
| [getView()](#getView--) | 获取要渲染的视图列列表（[GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)）。 |
| [getViewSettings()](#getViewSettings--) | 获取要渲染的视图 (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-)))。 |
| [isPortrait()](#isPortrait--) | 获取一个值，指示页面方向是否为纵向；如果页面方向为横向则返回 false。 |
| [setBarStyles(List&lt;BarStyle&gt; value)](#setBarStyles-java.util.List-com.aspose.tasks.BarStyle--) | 设置出现在项目视图中的 [BarStyle](../../com.aspose.tasks/barstyle) 类实例列表。 |
| [setCustomPageSize(Dimension2D value)](#setCustomPageSize-java.awt.geom.Dimension2D-) | 设置以点为单位的自定义页面大小（1 点 = 1/72 英寸）。 |
| [setDrawNonWorkingTime(boolean value)](#setDrawNonWorkingTime-boolean-) | 设置一个值，指示是否应绘制非工作时间（默认值为 TRUE）。 |
| [setEndDate(Date value)](#setEndDate-java.util.Date-) | 设置渲染结束的日期。 |
| [setFitContent(boolean value)](#setFitContent-boolean-) | 设置一个值，指示是否应增加行高以适应其内容。 |
| [setGridlines(List&lt;Gridline&gt; value)](#setGridlines-java.util.List-com.aspose.tasks.Gridline--) | 设置出现在项目视图中的 [Gridline](../../com.aspose.tasks/gridline) 列表。 |
| [setLegendDrawingOptions(int value)](#setLegendDrawingOptions-int-) | 设置一个值，定义如何渲染图例。 |
| [setLegendItems(PageLegendItem[] value)](#setLegendItems-com.aspose.tasks.PageLegendItem---) | 设置一个 PageLegendItem 数组，定义哪些条形应在页面图例中渲染。 |
| [setMarkCriticalTasks(boolean value)](#setMarkCriticalTasks-boolean-) | 设置一个值，指示关键任务是否应以红色显示（默认值为 FALSE）。 |
| [setNonWorkingTimeColor(Color value)](#setNonWorkingTimeColor-java.awt.Color-) | 设置非工作时间的颜色。 |
| [setPageSize(int value)](#setPageSize-int-) | 设置要渲染的页面大小（默认值为 PageSize.A4）。 |
| [setPortrait(boolean value)](#setPortrait-boolean-) | 设置一个值，指示页面方向是否为纵向；如果页面方向为横向则返回 false。 |
| [setPresentationFormat(int value)](#setPresentationFormat-int-) | 设置文档将被保存的 `PresentationFormat`（[getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-))。 |
| [setRenderToSinglePage(boolean value)](#setRenderToSinglePage-boolean-) | 设置一个值，指示在以图形格式保存项目时是否应将项目渲染为单页。 |
| [setRollUpGanttBars(boolean value)](#setRollUpGanttBars-boolean-) | 设置一个值，指示是否应标记汇总任务栏上的子任务。 |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | 设置渲染的起始日期。 |
| [setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value)](#setTaskLinkDrawingCallback-com.aspose.tasks.TaskLinkDrawingCallbackDelegate-) | 设置一个回调，可用于自定义任务链接渲染的某些方面。 |
| [setTextStyles(List&lt;TextStyle&gt; value)](#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--) | 设置在项目视图渲染期间应用的文本样式列表。 |
| [setTimescale(int value)](#setTimescale-int-) | 设置 `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) 值，用于控制在项目保存为图形格式时时间刻度（如果存在）如何渲染。 |
| [setTimescaleFitBehavior(int value)](#setTimescaleFitBehavior-int-) | 设置一种行为，定义如何将时间刻度的右端与页面末端对齐。 |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | 设置一个值，指示在渲染甘特图时是否应使用渐变画刷。 |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | 设置要渲染的视图列列表（[GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)）。 |
| [setViewSettings(View value)](#setViewSettings-com.aspose.tasks.View-) | 设置要渲染的视图 (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-)))。 |
### getBarStyles() {#getBarStyles--}
```
public final List<BarStyle> getBarStyles()
```


获取在项目视图中出现的 [BarStyle](../../com.aspose.tasks/barstyle) 类实例列表。

**Returns:**
java.util.List&lt;com.aspose.tasks.BarStyle&gt; - 出现在项目视图中的 [BarStyle](../../com.aspose.tasks/barstyle) 类实例列表。
### getCustomPageSize() {#getCustomPageSize--}
```
public final Dimension2D getCustomPageSize()
```


获取自定义页面尺寸（单位：点，1 点 = 1/72 英寸）。

**Returns:**
java.awt.geom.Dimension2D - 以点为单位的自定义页面尺寸（1 点 = 1/72 英寸）。
### getDrawNonWorkingTime() {#getDrawNonWorkingTime--}
```
public final boolean getDrawNonWorkingTime()
```


获取一个值，指示是否应绘制非工作时间（默认值为 TRUE）。

**Returns:**
boolean - 一个值，指示是否应绘制非工作时间（默认值为 TRUE）。
### getEndDate() {#getEndDate--}
```
public final Date getEndDate()
```


获取用于结束渲染的日期。

**Returns:**
java.util.Date - 用于结束渲染的日期。
### getFitContent() {#getFitContent--}
```
public final boolean getFitContent()
```


获取一个值，指示是否应增加行高以适应其内容。

**Returns:**
boolean - 一个值，指示是否应增加行高以适应其内容。
### getGridlines() {#getGridlines--}
```
public final List<Gridline> getGridlines()
```


获取在项目视图中出现的 [Gridline](../../com.aspose.tasks/gridline) 列表。

**Returns:**
java.util.List&lt;com.aspose.tasks.Gridline&gt; - 出现在项目视图中的 [Gridline](../../com.aspose.tasks/gridline) 列表。
### getLegendDrawingOptions() {#getLegendDrawingOptions--}
```
public final int getLegendDrawingOptions()
```


获取一个值，定义如何渲染图例。默认值为 LegendDrawingOptions.OnEveryPage。

仅在渲染甘特图视图时适用。

**Returns:**
int - 定义如何渲染图例的值。
### getLegendItems() {#getLegendItems--}
```
public final PageLegendItem[] getLegendItems()
```


获取一个 PageLegendItem 数组，定义哪些条形应在页面图例中渲染。如果为 null，则渲染默认项。

仅在渲染甘特图视图时适用。

**Returns:**
com.aspose.tasks.PageLegendItem[] - 一个 PageLegendItem 数组，定义哪些条形应在页面图例中渲染。
### getMarkCriticalTasks() {#getMarkCriticalTasks--}
```
public final boolean getMarkCriticalTasks()
```


获取一个值，指示是否应以红色显示关键任务（默认值为 FALSE）。

**Returns:**
boolean - 一个值，指示是否应以红色显示关键任务（默认值为 FALSE）。
### getNonWorkingTimeColor() {#getNonWorkingTimeColor--}
```
public final Color getNonWorkingTimeColor()
```


获取非工作时间的颜色。

**Returns:**
java.awt.Color - 非工作时间的颜色。
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


获取项目的页数。

**Returns:**
int - 项目的页数。
### getPageSize() {#getPageSize--}
```
public final int getPageSize()
```


获取要渲染的页面大小（默认值为 PageSize.A4）。

**Returns:**
int - 要渲染的页面大小（默认值为 PageSize.A4）。
### getPresentationFormat() {#getPresentationFormat--}
```
public final int getPresentationFormat()
```


获取文档将被保存的 `PresentationFormat`（[getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-))。

**Returns:**
int - 文档将保存的 `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-))。
### getRenderToSinglePage() {#getRenderToSinglePage--}
```
public final boolean getRenderToSinglePage()
```


获取一个值，指示在项目以图形格式保存时是否应将项目渲染为单页。页面大小将被更改，以便渲染的项目能够适配在一页上。

**Returns:**
boolean - 一个值，指示在项目以图形格式保存时是否应将项目渲染为单页。
### getRollUpGanttBars() {#getRollUpGanttBars--}
```
public final boolean getRollUpGanttBars()
```


获取一个值，指示是否应标记汇总任务栏上的子任务。对于子任务，Rollup 字段指示子任务甘特条的信息是否将汇总到汇总任务栏。对于汇总任务，Rollup 字段指示汇总任务栏是否显示已汇总的条。必须将汇总任务的 Rollup 字段设置为 Yes，才能将任何子任务汇总到它们上。

--------------------

仅在渲染甘特图视图时适用。

**Returns:**
boolean - 一个值，指示是否应标记汇总任务栏上的子任务。
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


获取渲染的起始日期。

**Returns:**
java.util.Date - 开始渲染的日期。
### getTaskLinkDrawingCallback() {#getTaskLinkDrawingCallback--}
```
public final TaskLinkDrawingCallbackDelegate getTaskLinkDrawingCallback()
```


获取一个回调，可用于自定义任务链接渲染的某些方面。

仅在渲染甘特图视图时适用。

**Returns:**
[TaskLinkDrawingCallbackDelegate](../../com.aspose.tasks/tasklinkdrawingcallbackdelegate) - a callback that can be used to customize some aspects of task links rendering.
### getTextStyles() {#getTextStyles--}
```
public final List<TextStyle> getTextStyles()
```


获取在项目视图渲染期间应用的文本样式列表。

--------------------

这些样式会覆盖使用 GanttCharView.setTextStyles 定义的样式。

**Returns:**
java.util.List&lt;com.aspose.tasks.TextStyle&gt; - 在项目视图渲染期间应用的文本样式列表。
### getTimescale() {#getTimescale--}
```
public final int getTimescale()
```


获取用于控制在项目保存为图形格式时时间刻度（如果存在）如何渲染的 `Timescale`（[getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) 值。

**Returns:**
int - 用于控制在项目保存为图形格式时时间尺度（如果存在）如何渲染的 `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) 值。
### getTimescaleFitBehavior() {#getTimescaleFitBehavior--}
```
public final int getTimescaleFitBehavior()
```


获取一种行为，定义如何将时间刻度的右端与页面末端对齐。

**Returns:**
int - 定义如何将时间尺度的右端与页面末端对齐的行为。
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


获取一个值，指示在渲染甘特图时是否应使用渐变画笔。

--------------------

仅在渲染甘特图视图时适用。

**Returns:**
boolean - 一个值，指示在渲染甘特图时是否应使用渐变画刷。
### getView() {#getView--}
```
public final ProjectView getView()
```


获取要渲染的视图列列表（[GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)）。如果未设置，则仅渲染任务 ID、任务名称、开始和结束。如果同时设置了 View 和 `ViewSettings`([getViewSettings()](../../com.aspose.tasks/saveoptions\#getViewSettings--)/[setViewSettings(View)](../../com.aspose.tasks/saveoptions\#setViewSettings-View-)) 属性，则 View 中的列会覆盖 ViewSettings 中的列。

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns to render ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)).
### getViewSettings() {#getViewSettings--}
```
public final View getViewSettings()
```


获取要渲染的视图（`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))）。您可以使用此选项显式指定应保存为 PDF、HTML 或图像格式的视图。如果设置了此属性，保存项目时将忽略 [PresentationFormat](../../com.aspose.tasks/presentationformat) 属性。视图应来自以下屏幕之一（(`Aspose.Tasks.View.Screen`([View.getScreen()](../../com.aspose.tasks/view\#getScreen--)/[View.setScreen(int)](../../com.aspose.tasks/view\#setScreen-int-)))）：（Gantt、TaskSheet、TaskUsage、ResourceSheet、ResourceUsage）

**Returns:**
[View](../../com.aspose.tasks/view) - a view (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) to render.
### isPortrait() {#isPortrait--}
```
public final boolean isPortrait()
```


获取一个值，指示页面方向是否为纵向；如果页面方向为横向则返回 false。

--------------------

当 SaveOptions.getPageSize() == PageSize.DefinedInView 时不适用。在这种情况下使用 [PageSettings.isPortrait()](../../com.aspose.tasks/pagesettings\#isPortrait--) 替代。当设置了 [getCustomPageSize()](../../com.aspose.tasks/saveoptions\#getCustomPageSize--) 时也不适用。

**Returns:**
boolean - 一个值，指示页面方向是否为纵向；如果页面方向为横向则返回 false。
### setBarStyles(List&lt;BarStyle&gt; value) {#setBarStyles-java.util.List-com.aspose.tasks.BarStyle--}
```
public final void setBarStyles(List<BarStyle> value)
```


设置出现在项目视图中的 [BarStyle](../../com.aspose.tasks/barstyle) 类实例列表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.BarStyle&gt; | 出现在项目视图中的 [BarStyle](../../com.aspose.tasks/barstyle) 类实例列表。 |

### setCustomPageSize(Dimension2D value) {#setCustomPageSize-java.awt.geom.Dimension2D-}
```
public final void setCustomPageSize(Dimension2D value)
```


设置以点为单位的自定义页面大小（1 点 = 1/72 英寸）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.awt.geom.Dimension2D | 以点为单位的自定义页面大小（1 点 = 1/72 英寸）。 |

### setDrawNonWorkingTime(boolean value) {#setDrawNonWorkingTime-boolean-}
```
public final void setDrawNonWorkingTime(boolean value)
```


设置一个值，指示是否应绘制非工作时间（默认值为 TRUE）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 一个值，指示是否应绘制非工作时间（默认值为 TRUE）。 |

### setEndDate(Date value) {#setEndDate-java.util.Date-}
```
public final void setEndDate(Date value)
```


设置渲染结束的日期。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date | 用于结束渲染的日期。 |

### setFitContent(boolean value) {#setFitContent-boolean-}
```
public final void setFitContent(boolean value)
```


设置一个值，指示是否应增加行高以适应其内容。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 一个值，指示是否应增加行高以适应其内容。 |

### setGridlines(List&lt;Gridline&gt; value) {#setGridlines-java.util.List-com.aspose.tasks.Gridline--}
```
public final void setGridlines(List<Gridline> value)
```


设置出现在项目视图中的 [Gridline](../../com.aspose.tasks/gridline) 列表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.Gridline&gt; | 出现在项目视图中的 [Gridline](../../com.aspose.tasks/gridline) 列表。 |

### setLegendDrawingOptions(int value) {#setLegendDrawingOptions-int-}
```
public final void setLegendDrawingOptions(int value)
```


设置一个值，定义图例的渲染方式。默认值为 LegendDrawingOptions.OnEveryPage。

仅在渲染甘特图视图时适用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 一个值，定义图例的渲染方式。 |

### setLegendItems(PageLegendItem[] value) {#setLegendItems-com.aspose.tasks.PageLegendItem---}
```
public final void setLegendItems(PageLegendItem[] value)
```


设置一个 PageLegendItem 数组，定义哪些条形应在页面图例中渲染。如果为 null，则渲染默认项。

仅在渲染甘特图视图时适用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [PageLegendItem\[\]](../../com.aspose.tasks/pagelegenditem) | 一个 PageLegendItem 数组，定义哪些条形应在页面图例中渲染。 |

### setMarkCriticalTasks(boolean value) {#setMarkCriticalTasks-boolean-}
```
public final void setMarkCriticalTasks(boolean value)
```


设置一个值，指示关键任务是否应以红色显示（默认值为 FALSE）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 一个值，指示是否应以红色显示关键任务（默认值为 FALSE）。 |

### setNonWorkingTimeColor(Color value) {#setNonWorkingTimeColor-java.awt.Color-}
```
public final void setNonWorkingTimeColor(Color value)
```


设置非工作时间的颜色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.awt.Color | 非工作时间颜色。 |

### setPageSize(int value) {#setPageSize-int-}
```
public final void setPageSize(int value)
```


设置要渲染的页面大小（默认值为 PageSize.A4）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 要渲染的页面大小（默认值为 PageSize.A4）。 |

### setPortrait(boolean value) {#setPortrait-boolean-}
```
public final void setPortrait(boolean value)
```


设置一个值，指示页面方向是否为纵向；如果页面方向为横向则返回 false。

--------------------

当 SaveOptions.PageSize == Visualization.PageSize.DefinedInView 时不适用。在这种情况下使用 [PageSettings.setPortrait(boolean)](../../com.aspose.tasks/pagesettings\#setPortrait-boolean-) 替代。当 [getCustomPageSize()](../../com.aspose.tasks/saveoptions\#getCustomPageSize--) 被设置时也不适用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 一个值，指示页面方向是否为纵向；如果页面方向为横向则返回 false。 |

### setPresentationFormat(int value) {#setPresentationFormat-int-}
```
public final void setPresentationFormat(int value)
```


设置文档将被保存的 `PresentationFormat`（[getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-))。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | int | 文档将保存的 `PresentationFormat`（[getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)）。 |

### setRenderToSinglePage(boolean value) {#setRenderToSinglePage-boolean-}
```
public final void setRenderToSinglePage(boolean value)
```


设置一个值，指示在项目以图形格式保存时是否应渲染为单页。页面大小将被更改，以便渲染的项目能够适合在一页上。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示在项目以图形格式保存时是否应渲染为单页的值。 |

### setRollUpGanttBars(boolean value) {#setRollUpGanttBars-boolean-}
```
public final void setRollUpGanttBars(boolean value)
```


设置一个值，指示是否应标记汇总任务栏上的子任务。对于子任务，Rollup 字段指示子任务甘特条的信息是否会汇总到汇总任务栏。对于汇总任务，Rollup 字段指示汇总任务栏是否显示汇总的条。必须将汇总任务的 Rollup 字段设置为 Yes，子任务才能汇总到它们。

--------------------

仅在渲染甘特图视图时适用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示是否应标记汇总任务栏上的子任务的值。 |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


设置渲染的起始日期。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.Date | 开始渲染的日期。 |

### setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value) {#setTaskLinkDrawingCallback-com.aspose.tasks.TaskLinkDrawingCallbackDelegate-}
```
public final void setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value)
```


设置一个回调，可用于自定义任务链接渲染的某些方面。

仅在渲染甘特图视图时适用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [TaskLinkDrawingCallbackDelegate](../../com.aspose.tasks/tasklinkdrawingcallbackdelegate) | 可用于自定义任务链接渲染某些方面的回调。 |

### setTextStyles(List&lt;TextStyle&gt; value) {#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--}
```
public final void setTextStyles(List<TextStyle> value)
```


设置在项目视图渲染期间应用的文本样式列表。

--------------------

这些样式会覆盖使用 GanttCharView.setTextStyles 定义的样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.util.List&lt;com.aspose.tasks.TextStyle&gt; | 在项目视图渲染期间应用的文本样式列表。 |

### setTimescale(int value) {#setTimescale-int-}
```
public final void setTimescale(int value)
```


设置 `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) 值，用于控制在项目保存为图形格式时时间刻度（如果存在）如何渲染。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | int | `Timescale`（[getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)）值，用于控制在项目保存为图形格式时时间刻度（如果存在）如何渲染。 |

### setTimescaleFitBehavior(int value) {#setTimescaleFitBehavior-int-}
```
public final void setTimescaleFitBehavior(int value)
```


设置一种行为，定义如何将时间刻度的右端与页面末端对齐。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int | 定义如何将时间刻度的右端与页面末端对齐的行为。 |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


设置一个值，指示在渲染甘特图时是否应使用渐变画刷。

--------------------

仅在渲染甘特图视图时适用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean | 指示在渲染甘特图时是否应使用渐变画刷的值。 |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


设置要渲染的视图列列表（[GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)）。如果未设置，则仅渲染任务 ID、任务名称、开始和结束。如果同时设置了 View 和 `ViewSettings`（[getViewSettings()](../../com.aspose.tasks/saveoptions\#getViewSettings--)/[setViewSettings(View)](../../com.aspose.tasks/saveoptions\#setViewSettings-View-)）属性，则 View 中的列覆盖 ViewSettings 中的列。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | 要渲染的视图列列表（[GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)）。 |

### setViewSettings(View value) {#setViewSettings-com.aspose.tasks.View-}
```
public final void setViewSettings(View value)
```


设置要渲染的视图（`View`（[getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-)））。您可以使用此选项明确指定应保存为 PDF、HTML 或图像格式的视图。如果设置了此属性，则在项目保存时会忽略 [PresentationFormat](../../com.aspose.tasks/presentationformat) 属性。视图应来自以下屏幕之一（（`Aspose.Tasks.View.Screen`（[View.getScreen()](../../com.aspose.tasks/view\#getScreen--)/[View.setScreen(int)](../../com.aspose.tasks/view\#setScreen-int-))））：（Gantt、TaskSheet、TaskUsage、ResourceSheet、ResourceUsage）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [View](../../com.aspose.tasks/view) | 要渲染的视图（`View`（[getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-)））。 |

