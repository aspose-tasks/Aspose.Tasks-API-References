---
title: Class ImageSaveOptions
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Saving.ImageSaveOptions class. Allows to specify additional options when rendering project pages to images
type: docs
weight: 1970
url: /net/aspose.tasks.saving/imagesaveoptions/
---
## ImageSaveOptions class

Allows to specify additional options when rendering project pages to images.

```csharp
public class ImageSaveOptions : SaveOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [ImageSaveOptions](imagesaveoptions/)(SaveFileFormat) | Initializes a new instance of the `ImageSaveOptions` class which can be used to save rendered images in TIFF, PNG, BMP or JPEG formats. |

## Properties

| Name | Description |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles/) { get; set; } | Gets or sets the list of the instances of the [`BarStyle`](../../aspose.tasks.visualization/barstyle/) class that appear in project view. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize/) { get; set; } | Gets or sets the custom page size in points (1 point = 1/72 of inch). |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime/) { get; set; } | Gets or sets a value indicating whether non-working time should be drawn (Default value is TRUE). |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate/) { get; set; } | Gets or sets a date to finish rendering to. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent/) { get; set; } | Gets or sets a value indicating whether row height should be increased to fit its content. |
| [FontSettings](../../aspose.tasks.saving/imagesaveoptions/fontsettings/) { get; } | Specifies font settings used when rendering project's view. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines/) { get; set; } | Gets or sets a list of [`Gridline`](../../aspose.tasks.visualization/gridline/) that appear in project view. |
| [HorizontalResolution](../../aspose.tasks.saving/imagesaveoptions/horizontalresolution/) { get; set; } | Gets or sets the horizontal resolution in dpi. |
| [IsPortrait](../../aspose.tasks.saving/saveoptions/isportrait/) { get; set; } | Gets or sets a value indicating whether the page orientation is portrait; returns false if the page orientation is landscape. |
| [JpegQuality](../../aspose.tasks.saving/imagesaveoptions/jpegquality/) { get; set; } | Gets or sets a JPEG quality. The allowed value range is 0..100. |
| [LegendDrawingOptions](../../aspose.tasks.saving/saveoptions/legenddrawingoptions/) { get; set; } | Gets or sets a value which define how to render a legend. Default value is LegendDrawingOptions.OnEveryPage. |
| [LegendItems](../../aspose.tasks.saving/saveoptions/legenditems/) { get; set; } | Gets or sets an array of PageLegendItem which define which bars should be rendered in page legend. If null, the default items are rendered. |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks/) { get; set; } | Gets or sets a value indicating whether critical tasks should be displayed in red color (Default value is FALSE). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor/) { get; set; } | Gets or sets the non-working time color. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount/) { get; } | Gets or sets the number of pages of project. |
| [Pages](../../aspose.tasks.saving/imagesaveoptions/pages/) { get; set; } | Gets or sets a list of page numbers to save when saving project layout to separate files. All pages will be saved if this list is empty. |
| [PageSavingCallback](../../aspose.tasks.saving/imagesaveoptions/pagesavingcallback/) { get; set; } | Gets or sets a user-defined callback which is used to get an output stream for each rendered page. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize/) { get; set; } | Gets or sets the size of page to be rendered (Default value is PageSize.A4). |
| [PixelFormat](../../aspose.tasks.saving/imagesaveoptions/pixelformat/) { get; set; } | Gets or sets the format of the color data for each pixel in the image. |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | Gets or sets the [`PresentationFormat`](../saveoptions/presentationformat/) in which the document will be saved. |
| [ReduceFooterGap](../../aspose.tasks.saving/imagesaveoptions/reducefootergap/) { get; set; } | Gets or sets a value indicating whether a gap between last task and the footer must be reduced. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage/) { get; set; } | Gets or sets a value indicating whether a project should be rendered to a single page when project is saved in graphical format. The page size will be changed so the rendered project can be fit on one page. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars/) { get; set; } | Gets or sets a value indicating whether subtasks on the summary task bar should be marked. For subtasks, the Rollup field indicates whether information on the subtask Gantt bars will be rolled up to the summary task bar. For summary tasks, the Rollup field indicates whether the summary task bar displays rolled up bars. You must have the Rollup field for summary tasks set to Yes for any subtasks to roll up to them. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Gets or sets the format in which the document will be saved if this save options object is used. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate/) { get; set; } | Gets or sets the date to start rendering from. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Gets or sets the comparer to sort tasks on Gantt chart and Task Sheet chart. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Gets or sets the condition which is used to filter tasks rendered on Gantt, Task Sheet and Task Usage charts. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles/) { get; set; } | Gets or sets the list of text styles that applied during rendering of a project view. |
| [TiffCompression](../../aspose.tasks.saving/imagesaveoptions/tiffcompression/) { get; set; } | Gets or sets the type of compression to apply when saving generated images to the TIFF format. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale/) { get; set; } | Gets or sets the [`Timescale`](../saveoptions/timescale/) value which is used to control how timescale (if present) is rendered when project is saved to graphical format. |
| [TimescaleFitBehavior](../../aspose.tasks.saving/saveoptions/timescalefitbehavior/) { get; set; } | Gets or sets a behavior which define how to align right end of the timescale with the page end. |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush/) { get; set; } | Gets or sets a value indicating whether gradient brush should be used when rendering Gantt Chart. |
| [VerticalResolution](../../aspose.tasks.saving/imagesaveoptions/verticalresolution/) { get; set; } | Gets or sets the vertical resolution in dpi. |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | Gets or sets a list of the view columns to render ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)). If not set then task ids, task names, start and finish are rendered only. If both View and [`ViewSettings`](../saveoptions/viewsettings/) properties are set, columns from View overrides columns from ViewSettings. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | Gets or sets a view ([`View`](../saveoptions/view/)) to render. You can use this options to explicitly specify which view should be saved to PDF, HTML or Image formats. If this property is set, [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) property is ignored when project is saved. View should be from one of the following screen (([`Screen`](../../aspose.tasks/view/screen/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |

## Examples

Shows how to save project into a stream as an image.

```csharp
var project = new Project();

using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var options = new ImageSaveOptions(SaveFileFormat.Png);

    // by using of ImageSaveOptions we save the project into image format
    project.Save(stream, options);
}
```

### See Also

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


