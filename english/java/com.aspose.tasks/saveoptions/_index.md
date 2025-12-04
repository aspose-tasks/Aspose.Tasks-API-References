---
title: SaveOptions
second_title: Aspose.Tasks for Java API Reference
description: This is an abstract base class for classes that allow the user to specify additional options when saving a project into a particular format.
type: docs
weight: 273
url: /java/com.aspose.tasks/saveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public abstract class SaveOptions extends SimpleSaveOptions
```

This is an abstract base class for classes that allow the user to specify additional options when saving a project into a particular format.

--------------------

An instance of any derived class from SaveOptions class is passed to the stream Save or string Save overloads for the user to define custom options when saving a document.
## Methods

| Method | Description |
| --- | --- |
| [getBarStyles()](#getBarStyles--) | Gets the list of the instances of the [BarStyle](../../com.aspose.tasks/barstyle) class that appear in project view. |
| [getCustomPageSize()](#getCustomPageSize--) | Gets the custom page size in points (1 point = 1/72 of inch). |
| [getDrawNonWorkingTime()](#getDrawNonWorkingTime--) | Gets a value indicating whether non-working time should be drawn (Default value is TRUE). |
| [getEndDate()](#getEndDate--) | Gets a date to finish rendering to. |
| [getFitContent()](#getFitContent--) | Gets a value indicating whether row height should be increased to fit its content. |
| [getFitTimescaleToEndOfPage()](#getFitTimescaleToEndOfPage--) | Gets whether a calendar section of a view should be rendered to the end (right side) of the last page. |
| [getGridlines()](#getGridlines--) | Gets a list of [Gridline](../../com.aspose.tasks/gridline) that appear in project view. |
| [getLegendDrawingOptions()](#getLegendDrawingOptions--) | Gets a value which define how to render a legend. |
| [getLegendItems()](#getLegendItems--) | Gets an array of PageLegendItem which define which bars should be rendered in page legend. |
| [getMarkCriticalTasks()](#getMarkCriticalTasks--) | Gets a value indicating whether critical tasks should be displayed in red color (Default value is FALSE). |
| [getNonWorkingTimeColor()](#getNonWorkingTimeColor--) | Gets the non-working time color. |
| [getPageCount()](#getPageCount--) | Gets the number of pages of project. |
| [getPageSize()](#getPageSize--) | Gets the size of page to be rendered (Default value is PageSize.A4). |
| [getPresentationFormat()](#getPresentationFormat--) | Gets the `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) in which the document will be saved. |
| [getRenderToSinglePage()](#getRenderToSinglePage--) | Gets a value indicating whether a project should be rendered to a single page when project is saved in graphical format. |
| [getRollUpGanttBars()](#getRollUpGanttBars--) | Gets a value indicating whether subtasks on the summary task bar should be marked. |
| [getStartDate()](#getStartDate--) | Gets the date to start rendering from. |
| [getTextStyles()](#getTextStyles--) | Gets the list of text styles that applied during rendering of a project view. |
| [getTimescale()](#getTimescale--) | Gets the `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) value which is used to control how timescale (if present) is rendered when project is saved to graphical format. |
| [getTimescaleFitBehavior()](#getTimescaleFitBehavior--) | Gets a behavior which define how to align right end of the timescale with the page end. |
| [getUseGradientBrush()](#getUseGradientBrush--) | Gets a value indicating whether gradient brush should be used when rendering Gantt Chart. |
| [getView()](#getView--) | Gets a list of the view columns to render ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |
| [getViewSettings()](#getViewSettings--) | Gets a view (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) to render. |
| [isPortrait()](#isPortrait--) | Gets a value indicating whether the page orientation is portrait; returns false if the page orientation is landscape. |
| [setBarStyles(List&lt;BarStyle&gt; value)](#setBarStyles-java.util.List-com.aspose.tasks.BarStyle--) | Sets the list of the instances of the [BarStyle](../../com.aspose.tasks/barstyle) class that appear in project view. |
| [setCustomPageSize(Dimension2D value)](#setCustomPageSize-java.awt.geom.Dimension2D-) | Sets the custom page size in points (1 point = 1/72 of inch). |
| [setDrawNonWorkingTime(boolean value)](#setDrawNonWorkingTime-boolean-) | Sets a value indicating whether non-working time should be drawn (Default value is TRUE). |
| [setEndDate(Date value)](#setEndDate-java.util.Date-) | Sets a date to finish rendering to. |
| [setFitContent(boolean value)](#setFitContent-boolean-) | Sets a value indicating whether row height should be increased to fit its content. |
| [setFitTimescaleToEndOfPage(boolean value)](#setFitTimescaleToEndOfPage-boolean-) | Sets whether a calendar section of a view should be rendered to the end (right side) of the last page. |
| [setGridlines(List&lt;Gridline&gt; value)](#setGridlines-java.util.List-com.aspose.tasks.Gridline--) | Sets a list of [Gridline](../../com.aspose.tasks/gridline) that appear in project view. |
| [setLegendDrawingOptions(int value)](#setLegendDrawingOptions-int-) | Sets a value which define how to render a legend. |
| [setLegendItems(PageLegendItem[] value)](#setLegendItems-com.aspose.tasks.PageLegendItem---) | Sets an array of PageLegendItem which define which bars should be rendered in page legend. |
| [setMarkCriticalTasks(boolean value)](#setMarkCriticalTasks-boolean-) | Sets a value indicating whether critical tasks should be displayed in red color (Default value is FALSE). |
| [setNonWorkingTimeColor(Color value)](#setNonWorkingTimeColor-java.awt.Color-) | Sets the non-working time color. |
| [setPageSize(int value)](#setPageSize-int-) | Sets the size of page to be rendered (Default value is PageSize.A4). |
| [setPortrait(boolean value)](#setPortrait-boolean-) | Sets a value indicating whether the page orientation is portrait; returns false if the page orientation is landscape. |
| [setPresentationFormat(int value)](#setPresentationFormat-int-) | Sets the `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) in which the document will be saved. |
| [setRenderToSinglePage(boolean value)](#setRenderToSinglePage-boolean-) | Sets a value indicating whether a project should be rendered to a single page when project is saved in graphical format. |
| [setRollUpGanttBars(boolean value)](#setRollUpGanttBars-boolean-) | Sets a value indicating whether subtasks on the summary task bar should be marked. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | Sets the date to start rendering from. |
| [setTextStyles(List&lt;TextStyle&gt; value)](#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--) | Sets the list of text styles that applied during rendering of a project view. |
| [setTimescale(int value)](#setTimescale-int-) | Sets the `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) value which is used to control how timescale (if present) is rendered when project is saved to graphical format. |
| [setTimescaleFitBehavior(int value)](#setTimescaleFitBehavior-int-) | Sets a behavior which define how to align right end of the timescale with the page end. |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | Sets a value indicating whether gradient brush should be used when rendering Gantt Chart. |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | Sets a list of the view columns to render ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |
| [setViewSettings(View value)](#setViewSettings-com.aspose.tasks.View-) | Sets a view (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) to render. |
### getBarStyles() {#getBarStyles--}
```
public final List<BarStyle> getBarStyles()
```


Gets the list of the instances of the [BarStyle](../../com.aspose.tasks/barstyle) class that appear in project view.

**Returns:**
java.util.List&lt;com.aspose.tasks.BarStyle&gt; - the list of the instances of the [BarStyle](../../com.aspose.tasks/barstyle) class that appear in project view.
### getCustomPageSize() {#getCustomPageSize--}
```
public final Dimension2D getCustomPageSize()
```


Gets the custom page size in points (1 point = 1/72 of inch).

**Returns:**
java.awt.geom.Dimension2D - the custom page size in points (1 point = 1/72 of inch).
### getDrawNonWorkingTime() {#getDrawNonWorkingTime--}
```
public final boolean getDrawNonWorkingTime()
```


Gets a value indicating whether non-working time should be drawn (Default value is TRUE).

**Returns:**
boolean - a value indicating whether non-working time should be drawn (Default value is TRUE).
### getEndDate() {#getEndDate--}
```
public final Date getEndDate()
```


Gets a date to finish rendering to.

**Returns:**
java.util.Date - a date to finish rendering to.
### getFitContent() {#getFitContent--}
```
public final boolean getFitContent()
```


Gets a value indicating whether row height should be increased to fit its content.

**Returns:**
boolean - a value indicating whether row height should be increased to fit its content.
### getFitTimescaleToEndOfPage() {#getFitTimescaleToEndOfPage--}
```
public final boolean getFitTimescaleToEndOfPage()
```


Gets whether a calendar section of a view should be rendered to the end (right side) of the last page. If value is false, calendar section is rendered exactly to EndDate, even there is an empty space on a page.

**Returns:**
boolean - whether a calendar section of a view should be rendered to the end (right side) of the last page.
### getGridlines() {#getGridlines--}
```
public final List<Gridline> getGridlines()
```


Gets a list of [Gridline](../../com.aspose.tasks/gridline) that appear in project view.

**Returns:**
java.util.List&lt;com.aspose.tasks.Gridline&gt; - a list of [Gridline](../../com.aspose.tasks/gridline) that appear in project view.
### getLegendDrawingOptions() {#getLegendDrawingOptions--}
```
public final int getLegendDrawingOptions()
```


Gets a value which define how to render a legend. Default value is LegendDrawingOptions.OnEveryPage.

Is only applicable when Gantt chart view is rendered.

**Returns:**
int - a value which define how to render a legend.
### getLegendItems() {#getLegendItems--}
```
public final PageLegendItem[] getLegendItems()
```


Gets an array of PageLegendItem which define which bars should be rendered in page legend. If null, the default items are rendered.

Is only applicable when Gantt chart view is rendered.

**Returns:**
com.aspose.tasks.PageLegendItem[] - an array of PageLegendItem which define which bars should be rendered in page legend.
### getMarkCriticalTasks() {#getMarkCriticalTasks--}
```
public final boolean getMarkCriticalTasks()
```


Gets a value indicating whether critical tasks should be displayed in red color (Default value is FALSE).

**Returns:**
boolean - a value indicating whether critical tasks should be displayed in red color (Default value is FALSE).
### getNonWorkingTimeColor() {#getNonWorkingTimeColor--}
```
public final Color getNonWorkingTimeColor()
```


Gets the non-working time color.

**Returns:**
java.awt.Color - the non-working time color.
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Gets the number of pages of project.

**Returns:**
int - the number of pages of project.
### getPageSize() {#getPageSize--}
```
public final int getPageSize()
```


Gets the size of page to be rendered (Default value is PageSize.A4).

**Returns:**
int - the size of page to be rendered (Default value is PageSize.A4).
### getPresentationFormat() {#getPresentationFormat--}
```
public final int getPresentationFormat()
```


Gets the `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) in which the document will be saved.

**Returns:**
int - the `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) in which the document will be saved.
### getRenderToSinglePage() {#getRenderToSinglePage--}
```
public final boolean getRenderToSinglePage()
```


Gets a value indicating whether a project should be rendered to a single page when project is saved in graphical format. The page size will be changed so the rendered project can be fit on one page.

**Returns:**
boolean - a value indicating whether a project should be rendered to a single page when project is saved in graphical format.
### getRollUpGanttBars() {#getRollUpGanttBars--}
```
public final boolean getRollUpGanttBars()
```


Gets a value indicating whether subtasks on the summary task bar should be marked. For subtasks, the Rollup field indicates whether information on the subtask Gantt bars will be rolled up to the summary task bar. For summary tasks, the Rollup field indicates whether the summary task bar displays rolled up bars. You must have the Rollup field for summary tasks set to Yes for any subtasks to roll up to them.

--------------------

Is only applicable when Gantt chart view is rendered.

**Returns:**
boolean - a value indicating whether subtasks on the summary task bar should be marked.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


Gets the date to start rendering from.

**Returns:**
java.util.Date - the date to start rendering from.
### getTextStyles() {#getTextStyles--}
```
public final List<TextStyle> getTextStyles()
```


Gets the list of text styles that applied during rendering of a project view.

--------------------

These styles override styles defined with GanttCharView.setTextStyles.

**Returns:**
java.util.List&lt;com.aspose.tasks.TextStyle&gt; - the list of text styles that applied during rendering of a project view.
### getTimescale() {#getTimescale--}
```
public final int getTimescale()
```


Gets the `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) value which is used to control how timescale (if present) is rendered when project is saved to graphical format.

**Returns:**
int - the `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) value which is used to control how timescale (if present) is rendered when project is saved to graphical format.
### getTimescaleFitBehavior() {#getTimescaleFitBehavior--}
```
public final int getTimescaleFitBehavior()
```


Gets a behavior which define how to align right end of the timescale with the page end.

**Returns:**
int - a behavior which define how to align right end of the timescale with the page end.
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


Gets a value indicating whether gradient brush should be used when rendering Gantt Chart.

--------------------

Is only applicable when Gantt chart view is rendered.

**Returns:**
boolean - a value indicating whether gradient brush should be used when rendering Gantt Chart.
### getView() {#getView--}
```
public final ProjectView getView()
```


Gets a list of the view columns to render ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). If not set then task ids, task names, start and finish are rendered only. If both View and `ViewSettings`([getViewSettings()](../../com.aspose.tasks/saveoptions\#getViewSettings--)/[setViewSettings(View)](../../com.aspose.tasks/saveoptions\#setViewSettings-View-)) properties are set, columns from View overrides columns from ViewSettings.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns to render ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)).
### getViewSettings() {#getViewSettings--}
```
public final View getViewSettings()
```


Gets a view (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) to render. You can use this options to explicitly specify which view should be saved to PDF, HTML or Image formats. If this property is set, [PresentationFormat](../../com.aspose.tasks/presentationformat) property is ignored when project is saved. View should be from one of the following screen ((`Aspose.Tasks.View.Screen`([View.getScreen()](../../com.aspose.tasks/view\#getScreen--)/[View.setScreen(int)](../../com.aspose.tasks/view\#setScreen-int-)))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage)

**Returns:**
[View](../../com.aspose.tasks/view) - a view (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) to render.
### isPortrait() {#isPortrait--}
```
public final boolean isPortrait()
```


Gets a value indicating whether the page orientation is portrait; returns false if the page orientation is landscape.

--------------------

Is not applicable when SaveOptions.getPageSize() == PageSize.DefinedInView. In this case [PageSettings.isPortrait()](../../com.aspose.tasks/pagesettings\#isPortrait--) is used instead. Is not applicable when [getCustomPageSize()](../../com.aspose.tasks/saveoptions\#getCustomPageSize--) is set.

**Returns:**
boolean - a value indicating whether the page orientation is portrait; returns false if the page orientation is landscape.
### setBarStyles(List&lt;BarStyle&gt; value) {#setBarStyles-java.util.List-com.aspose.tasks.BarStyle--}
```
public final void setBarStyles(List<BarStyle> value)
```


Sets the list of the instances of the [BarStyle](../../com.aspose.tasks/barstyle) class that appear in project view.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.BarStyle&gt; | the list of the instances of the [BarStyle](../../com.aspose.tasks/barstyle) class that appear in project view. |

### setCustomPageSize(Dimension2D value) {#setCustomPageSize-java.awt.geom.Dimension2D-}
```
public final void setCustomPageSize(Dimension2D value)
```


Sets the custom page size in points (1 point = 1/72 of inch).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.awt.geom.Dimension2D | the custom page size in points (1 point = 1/72 of inch). |

### setDrawNonWorkingTime(boolean value) {#setDrawNonWorkingTime-boolean-}
```
public final void setDrawNonWorkingTime(boolean value)
```


Sets a value indicating whether non-working time should be drawn (Default value is TRUE).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether non-working time should be drawn (Default value is TRUE). |

### setEndDate(Date value) {#setEndDate-java.util.Date-}
```
public final void setEndDate(Date value)
```


Sets a date to finish rendering to.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a date to finish rendering to. |

### setFitContent(boolean value) {#setFitContent-boolean-}
```
public final void setFitContent(boolean value)
```


Sets a value indicating whether row height should be increased to fit its content.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether row height should be increased to fit its content. |

### setFitTimescaleToEndOfPage(boolean value) {#setFitTimescaleToEndOfPage-boolean-}
```
public final void setFitTimescaleToEndOfPage(boolean value)
```


Sets whether a calendar section of a view should be rendered to the end (right side) of the last page. If value is false, calendar section is rendered exactly to EndDate, even there is an empty space on a page.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | whether a calendar section of a view should be rendered to the end (right side) of the last page. |

### setGridlines(List&lt;Gridline&gt; value) {#setGridlines-java.util.List-com.aspose.tasks.Gridline--}
```
public final void setGridlines(List<Gridline> value)
```


Sets a list of [Gridline](../../com.aspose.tasks/gridline) that appear in project view.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.Gridline&gt; | a list of [Gridline](../../com.aspose.tasks/gridline) that appear in project view. |

### setLegendDrawingOptions(int value) {#setLegendDrawingOptions-int-}
```
public final void setLegendDrawingOptions(int value)
```


Sets a value which define how to render a legend. Default value is LegendDrawingOptions.OnEveryPage.

Is only applicable when Gantt chart view is rendered.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value which define how to render a legend. |

### setLegendItems(PageLegendItem[] value) {#setLegendItems-com.aspose.tasks.PageLegendItem---}
```
public final void setLegendItems(PageLegendItem[] value)
```


Sets an array of PageLegendItem which define which bars should be rendered in page legend. If null, the default items are rendered.

Is only applicable when Gantt chart view is rendered.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PageLegendItem\[\]](../../com.aspose.tasks/pagelegenditem) | an array of PageLegendItem which define which bars should be rendered in page legend. |

### setMarkCriticalTasks(boolean value) {#setMarkCriticalTasks-boolean-}
```
public final void setMarkCriticalTasks(boolean value)
```


Sets a value indicating whether critical tasks should be displayed in red color (Default value is FALSE).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether critical tasks should be displayed in red color (Default value is FALSE). |

### setNonWorkingTimeColor(Color value) {#setNonWorkingTimeColor-java.awt.Color-}
```
public final void setNonWorkingTimeColor(Color value)
```


Sets the non-working time color.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.awt.Color | the non-working time color. |

### setPageSize(int value) {#setPageSize-int-}
```
public final void setPageSize(int value)
```


Sets the size of page to be rendered (Default value is PageSize.A4).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the size of page to be rendered (Default value is PageSize.A4). |

### setPortrait(boolean value) {#setPortrait-boolean-}
```
public final void setPortrait(boolean value)
```


Sets a value indicating whether the page orientation is portrait; returns false if the page orientation is landscape.

--------------------

Is not applicable when SaveOptions.PageSize == Visualization.PageSize.DefinedInView. In this case [PageSettings.setPortrait(boolean)](../../com.aspose.tasks/pagesettings\#setPortrait-boolean-) is used instead. Is not applicable when [getCustomPageSize()](../../com.aspose.tasks/saveoptions\#getCustomPageSize--) is set.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether the page orientation is portrait; returns false if the page orientation is landscape. |

### setPresentationFormat(int value) {#setPresentationFormat-int-}
```
public final void setPresentationFormat(int value)
```


Sets the `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) in which the document will be saved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) in which the document will be saved. |

### setRenderToSinglePage(boolean value) {#setRenderToSinglePage-boolean-}
```
public final void setRenderToSinglePage(boolean value)
```


Sets a value indicating whether a project should be rendered to a single page when project is saved in graphical format. The page size will be changed so the rendered project can be fit on one page.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether a project should be rendered to a single page when project is saved in graphical format. |

### setRollUpGanttBars(boolean value) {#setRollUpGanttBars-boolean-}
```
public final void setRollUpGanttBars(boolean value)
```


Sets a value indicating whether subtasks on the summary task bar should be marked. For subtasks, the Rollup field indicates whether information on the subtask Gantt bars will be rolled up to the summary task bar. For summary tasks, the Rollup field indicates whether the summary task bar displays rolled up bars. You must have the Rollup field for summary tasks set to Yes for any subtasks to roll up to them.

--------------------

Is only applicable when Gantt chart view is rendered.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether subtasks on the summary task bar should be marked. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


Sets the date to start rendering from.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | the date to start rendering from. |

### setTextStyles(List&lt;TextStyle&gt; value) {#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--}
```
public final void setTextStyles(List<TextStyle> value)
```


Sets the list of text styles that applied during rendering of a project view.

--------------------

These styles override styles defined with GanttCharView.setTextStyles.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.TextStyle&gt; | the list of text styles that applied during rendering of a project view. |

### setTimescale(int value) {#setTimescale-int-}
```
public final void setTimescale(int value)
```


Sets the `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) value which is used to control how timescale (if present) is rendered when project is saved to graphical format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) value which is used to control how timescale (if present) is rendered when project is saved to graphical format. |

### setTimescaleFitBehavior(int value) {#setTimescaleFitBehavior-int-}
```
public final void setTimescaleFitBehavior(int value)
```


Sets a behavior which define how to align right end of the timescale with the page end.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a behavior which define how to align right end of the timescale with the page end. |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


Sets a value indicating whether gradient brush should be used when rendering Gantt Chart.

--------------------

Is only applicable when Gantt chart view is rendered.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether gradient brush should be used when rendering Gantt Chart. |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


Sets a list of the view columns to render ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). If not set then task ids, task names, start and finish are rendered only. If both View and `ViewSettings`([getViewSettings()](../../com.aspose.tasks/saveoptions\#getViewSettings--)/[setViewSettings(View)](../../com.aspose.tasks/saveoptions\#setViewSettings-View-)) properties are set, columns from View overrides columns from ViewSettings.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | a list of the view columns to render ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |

### setViewSettings(View value) {#setViewSettings-com.aspose.tasks.View-}
```
public final void setViewSettings(View value)
```


Sets a view (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) to render. You can use this options to explicitly specify which view should be saved to PDF, HTML or Image formats. If this property is set, [PresentationFormat](../../com.aspose.tasks/presentationformat) property is ignored when project is saved. View should be from one of the following screen ((`Aspose.Tasks.View.Screen`([View.getScreen()](../../com.aspose.tasks/view\#getScreen--)/[View.setScreen(int)](../../com.aspose.tasks/view\#setScreen-int-)))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [View](../../com.aspose.tasks/view) | a view (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) to render. |

