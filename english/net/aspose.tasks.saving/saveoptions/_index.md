---
title: SaveOptions
second_title: Aspose.Tasks for .NET API Reference
description: This is an abstract base class for classes that allow the user to specify additional options when saving a project into a particular format.
type: docs
weight: 1980
url: /net/aspose.tasks.saving/saveoptions/
---
## SaveOptions class

This is an abstract base class for classes that allow the user to specify additional options when saving a project into a particular format.

```csharp
public abstract class SaveOptions
```

## Properties

| Name | Description |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles) { get; set; } | Gets or sets the list of the instances of the [`BarStyle`](../../aspose.tasks.visualization/barstyle) class that appear in project view. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize) { get; set; } | Gets or sets the custom page size in points (1 point = 1/72 of inch). |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime) { get; set; } | Gets or sets a value indicating whether non-working time should be drawn (Default value is TRUE). |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate) { get; set; } | Gets or sets a date to finish rendering to. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent) { get; set; } | Gets or sets a value indicating whether row height should be increased to fit its content. |
| [FitTimescaleToEndOfPage](../../aspose.tasks.saving/saveoptions/fittimescaletoendofpage) { get; set; } | Gets or sets whether a calendar section of a view should be rendered to the end (right side) of the last page. If value is false, calendar section is rendered exactly to EndDate, even there is an empty space on a page. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines) { get; set; } | Gets or sets a list of [`Gridline`](../../aspose.tasks.visualization/gridline) that appear in project view. |
| [LegendOnEachPage](../../aspose.tasks.saving/saveoptions/legendoneachpage) { get; set; } | Gets or sets a value indicating whether legend should be shown on each page (Default value is TRUE). |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks) { get; set; } | Gets or sets a value indicating whether critical tasks should be displayed in red color (Default value is FALSE). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor) { get; set; } | Gets or sets the non-working time color. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount) { get; } | Gets or sets the number of pages of project. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize) { get; set; } | Gets or sets the size of page to be rendered (Default value is PageSize.A4). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat) { get; set; } | Gets or sets the [`PresentationFormat`](./presentationformat) in which the document will be saved. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage) { get; set; } | Gets or sets a value indicating whether a project should be rendered to a single page when project is saved in graphical format. The page size will be changed so the rendered project can be fit on one page. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars) { get; set; } | Gets or sets a value indicating whether subtasks on the summary task bar should be marked. For subtasks, the Rollup field indicates whether information on the subtask Gantt bars will be rolled up to the summary task bar. For summary tasks, the Rollup field indicates whether the summary task bar displays rolled up bars. You must have the Rollup field for summary tasks set to Yes for any subtasks to roll up to them. |
| [SaveFormat](../../aspose.tasks.saving/saveoptions/saveformat) { get; } | Gets or sets the format in which the document will be saved if this save options object is used. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate) { get; set; } | Gets or sets the date to start rendering from. |
| [TasksComparer](../../aspose.tasks.saving/saveoptions/taskscomparer) { get; set; } | Gets or sets the comparer to sort tasks on Gantt chart and Task Sheet chart. |
| [TasksFilter](../../aspose.tasks.saving/saveoptions/tasksfilter) { get; set; } | Gets or sets the condition which is used to filter tasks rendered on Gantt, Task Sheet and Task Usage charts. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles) { get; set; } | Gets or sets the list of the instances of the [`TextStyle`](../../aspose.tasks.visualization/textstyle) class that appear in project view. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale) { get; set; } | Gets or sets the [`Timescale`](./timescale) value which is used to control how timescale (if present) is rendered when project is saved to graphical format. |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush) { get; set; } | Gets or sets a value indicating whether gradient brush should be used when rendering Gantt Chart. |
| [View](../../aspose.tasks.saving/saveoptions/view) { get; set; } | Gets or sets a list of the view columns to render ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn)). If not set then task ids, task names, start and finish are rendered only. If both View and [`ViewSettings`](./viewsettings) properties are set, columns from View overrides columns from ViewSettings. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings) { get; set; } | Gets or sets a view ([`View`](./view)) to render. You can use this options to explicitly specify which view should be saved to PDF, HTML or Image formats. If this property is set, [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat) property is ignored when project is saved. View should be from one of the following screen (([`Screen`](../../aspose.tasks/view/screen))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |

### Remarks

An instance of any derived class from SaveOptions class is passed to the stream Save or string Save overloads for the user to define custom options when saving a document.

### Examples

Shows how to set the option whether row height should be increased to fit its content.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    // Set option fit content to true
    FitContent = true,
    Timescale = Timescale.Months,
    PresentationFormat = PresentationFormat.TaskUsage
};
project.Save(OutDir + "FitContentsToCellSize_out.pdf", options);
```

### See Also

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving)
* assembly [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
