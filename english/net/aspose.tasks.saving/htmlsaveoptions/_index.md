---
title: HtmlSaveOptions
second_title: Aspose.Tasks for .NET API Reference
description: Allows to specify additional options when rendering project pages to HTML.
type: docs
weight: 1740
url: /net/aspose.tasks.saving/htmlsaveoptions/
---
## HtmlSaveOptions class

Allows to specify additional options when rendering project pages to HTML.

```csharp
public class HtmlSaveOptions : SaveOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions)() | Initializes a new instance of the [`HtmlSaveOptions`](../htmlsaveoptions) class. |

## Properties

| Name | Description |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles) { get; set; } | Gets or sets the list of the instances of the [`BarStyle`](../../aspose.tasks.visualization/barstyle) class that appear in project view. |
| [CssSavingCallback](../../aspose.tasks.saving/htmlsaveoptions/csssavingcallback) { get; set; } | Gets or sets the callback that is called to create resource to store CSS. |
| [CssStylePrefix](../../aspose.tasks.saving/htmlsaveoptions/cssstyleprefix) { get; set; } | Gets or sets CSS style prefix. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize) { get; set; } | Gets or sets the custom page size in points (1 point = 1/72 of inch). |
| [DefaultFontName](../../aspose.tasks.saving/htmlsaveoptions/defaultfontname) { get; set; } | Gets or sets the default font for rendering. |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime) { get; set; } | Gets or sets a value indicating whether non-working time should be drawn (Default value is TRUE). |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate) { get; set; } | Gets or sets a date to finish rendering to. |
| [ExportCss](../../aspose.tasks.saving/htmlsaveoptions/exportcss) { get; set; } | Gets or sets the way CSS are exported. |
| [ExportFonts](../../aspose.tasks.saving/htmlsaveoptions/exportfonts) { get; set; } | Gets or sets the way fonts are exported. |
| [ExportImages](../../aspose.tasks.saving/htmlsaveoptions/exportimages) { get; set; } | Gets or sets the way images are exported. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent) { get; set; } | Gets or sets a value indicating whether row height should be increased to fit its content. |
| [FontFaceTypes](../../aspose.tasks.saving/htmlsaveoptions/fontfacetypes) { get; set; } | Gets or sets the font face types. |
| [FontResolveCallback](../../aspose.tasks.saving/htmlsaveoptions/fontresolvecallback) { get; set; } | Gets or sets a callback which can be used to customize resolved fonts. |
| [FontSavingCallback](../../aspose.tasks.saving/htmlsaveoptions/fontsavingcallback) { get; set; } | Gets or sets the callback that is called to create resource to store font. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines) { get; set; } | Gets or sets a list of [`Gridline`](../../aspose.tasks.visualization/gridline) that appear in project view. |
| [ImageSavingCallback](../../aspose.tasks.saving/htmlsaveoptions/imagesavingcallback) { get; set; } | Gets or sets the callback that is called to create resource to store font. |
| [IncludeProjectNameInPageHeader](../../aspose.tasks.saving/htmlsaveoptions/includeprojectnameinpageheader) { get; set; } | Gets or sets a value indicating whether to include project name in HTML page header. |
| [IncludeProjectNameInTitle](../../aspose.tasks.saving/htmlsaveoptions/includeprojectnameintitle) { get; set; } | Gets or sets a value indicating whether to include project name in HTML title. |
| [LegendOnEachPage](../../aspose.tasks.saving/saveoptions/legendoneachpage) { get; set; } | Gets or sets a value indicating whether legend should be shown on each page (Default value is TRUE). |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks) { get; set; } | Gets or sets a value indicating whether critical tasks should be displayed in red color (Default value is FALSE). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor) { get; set; } | Gets or sets the non-working time color. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount) { get; } | Gets or sets the number of pages of project. |
| [Pages](../../aspose.tasks.saving/htmlsaveoptions/pages) { get; set; } | Gets or sets a list of page numbers to save when rendering project layout. All project pages will be saved if this list is empty. |
| [PageSavingCallback](../../aspose.tasks.saving/htmlsaveoptions/pagesavingcallback) { get; set; } | Gets or sets a user-defined callback which is used to get an output stream for each rendered page. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize) { get; set; } | Gets or sets the size of page to be rendered (Default value is PageSize.A4). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat) { get; set; } | Gets or sets the [`PresentationFormat`](../saveoptions/presentationformat) in which the document will be saved. |
| [ReduceFooterGap](../../aspose.tasks.saving/htmlsaveoptions/reducefootergap) { get; set; } | Gets or sets a value indicating whether a gap between last task and the footer must be reduced. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage) { get; set; } | Gets or sets a value indicating whether a project should be rendered to a single page when project is saved in graphical format. The page size will be changed so the rendered project can be fit on one page. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars) { get; set; } | Gets or sets a value indicating whether subtasks on the summary task bar should be marked. For subtasks, the Rollup field indicates whether information on the subtask Gantt bars will be rolled up to the summary task bar. For summary tasks, the Rollup field indicates whether the summary task bar displays rolled up bars. You must have the Rollup field for summary tasks set to Yes for any subtasks to roll up to them. |
| [SaveFormat](../../aspose.tasks.saving/saveoptions/saveformat) { get; } | Gets or sets the format in which the document will be saved if this save options object is used. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate) { get; set; } | Gets or sets the date to start rendering from. |
| [TasksComparer](../../aspose.tasks.saving/saveoptions/taskscomparer) { get; set; } | Gets or sets the comparer to sort tasks on Gantt chart and Task Sheet chart. |
| [TasksFilter](../../aspose.tasks.saving/saveoptions/tasksfilter) { get; set; } | Gets or sets the condition which is used to filter tasks rendered on Gantt, Task Sheet and Task Usage charts. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles) { get; set; } | Gets or sets the list of the instances of the [`TextStyle`](../../aspose.tasks.visualization/textstyle) class that appear in project view. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale) { get; set; } | Gets or sets the [`Timescale`](../saveoptions/timescale) value which is used to control how timescale (if present) is rendered when project is saved to graphical format. |
| override [UseGradientBrush](../../aspose.tasks.saving/htmlsaveoptions/usegradientbrush) { get; set; } | Gets or sets a value indicating whether to use gradient brush when rendering project layout. Currently using of gradient brush is not supported when rendering to HTML. |
| [UseProjectDefaultFont](../../aspose.tasks.saving/htmlsaveoptions/useprojectdefaultfont) { get; set; } | Gets or sets a value indicating whether the default font must be used for rendering. |
| [View](../../aspose.tasks.saving/saveoptions/view) { get; set; } | Gets or sets a list of the view columns to render ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn)). If not set then task ids, task names, start and finish are rendered only. If both View and [`ViewSettings`](../saveoptions/viewsettings) properties are set, columns from View overrides columns from ViewSettings. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings) { get; set; } | Gets or sets a view ([`View`](../saveoptions/view)) to render. You can use this options to explicitly specify which view should be saved to PDF, HTML or Image formats. If this property is set, [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat) property is ignored when project is saved. View should be from one of the following screen (([`Screen`](../../aspose.tasks/view/screen))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |

### See Also

* class [SaveOptions](../saveoptions)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving)
* assembly [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
