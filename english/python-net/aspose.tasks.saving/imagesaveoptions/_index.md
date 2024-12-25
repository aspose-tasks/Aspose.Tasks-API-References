---
title: ImageSaveOptions
second_title: Aspose.Tasks for Python via .NET API Reference
description: 
type: docs
weight: 40
url: /python-net/aspose.tasks.saving/imagesaveoptions/
---

## ImageSaveOptions class

Allows to specify additional options when rendering project pages to images.

The ImageSaveOptions type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|ImageSaveOptions(save_format)|Initializes a new instance of the [ImageSaveOptions](/tasks/python-net/aspose.tasks.saving/imagesaveoptions/) class which can be used to save rendered images in TIFF, PNG, BMP or JPEG formats.|
## Properties
| Name | Description |
| :- | :- |
|save_format|  |
|bar_styles|Gets or sets the list of the instances of the [BarStyle](/tasks/python-net/aspose.tasks.visualization/barstyle/) class that appear in project view.|
|draw_non_working_time|Gets or sets a value indicating whether non-working time should be drawn (Default value is TRUE).|
|end_date|Gets or sets a date to finish rendering to.|
|fit_timescale_to_end_of_page|Gets or sets whether a calendar section of a view should be rendered to the end (right side) of the last page.<br/>            If value is false, calendar section is rendered exactly to EndDate, even there is an empty space on a page.|
|fit_content|Gets or sets a value indicating whether row height should be increased to fit its content.|
|gridlines|Gets or sets a list of [Gridline](/tasks/python-net/aspose.tasks.visualization/gridline/) that appear in project view.|
|legend_drawing_options|Gets or sets a value which define how to render a legend. Default value is LegendDrawingOptions.OnEveryPage.|
|mark_critical_tasks|Gets or sets a value indicating whether critical tasks should be displayed in red color (Default value is FALSE).|
|non_working_time_color|Gets or sets the non-working time color.|
|page_count|Gets or sets the number of pages of project.|
|page_size|Gets or sets the size of page to be rendered (Default value is PageSize.A4).|
|is_portrait|Gets or sets a value indicating whether the page orientation is portrait; returns false if the page orientation is landscape.|
|presentation_format|Gets or sets the [presentation_format](/tasks/python-net/aspose.tasks.saving/saveoptions/) in which the document will be saved.|
|roll_up_gantt_bars|Gets or sets a value indicating whether subtasks on the summary task bar should be marked.<br/>            For subtasks, the Rollup field indicates whether information on the subtask Gantt bars will be rolled up to the summary task bar.<br/>            For summary tasks, the Rollup field indicates whether the summary task bar displays rolled up bars.<br/>            You must have the Rollup field for summary tasks set to Yes for any subtasks to roll up to them.|
|start_date|Gets or sets the date to start rendering from.|
|text_styles|Gets or sets the list of text styles that applied during rendering of a project view.|
|timescale|Gets or sets the [timescale](/tasks/python-net/aspose.tasks.saving/saveoptions/) value which is used to control how timescale (if present) is rendered when project is saved to graphical format.|
|use_gradient_brush|Gets or sets a value indicating whether gradient brush should be used when rendering Gantt Chart.|
|view|Gets or sets a list of the view columns to render ([GanttChartColumn](/tasks/python-net/aspose.tasks.visualization/ganttchartcolumn/)).<br/>            If not set then task ids, task names, start and finish are rendered only.<br/>            If both View and [view_settings](/tasks/python-net/aspose.tasks.saving/saveoptions/) properties are set, columns from View overrides columns from ViewSettings.|
|view_settings|Gets or sets a view ([view](/tasks/python-net/aspose.tasks.saving/saveoptions/)) to render. You can use this options to explicitly specify which view should be saved to PDF, HTML or Image formats.<br/>            If this property is set, [PresentationFormat](/tasks/python-net/aspose.tasks.visualization/presentationformat/) property is ignored when project is saved.<br/>            View should be from one of the following screen (([screen](/tasks/python-net/aspose.tasks/view/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage)|
|custom_page_size|Gets or sets the custom page size in points (1 point = 1/72 of inch).|
|render_to_single_page|Gets or sets a value indicating whether a project should be rendered to a single page<br/>            when project is saved in graphical format.<br/>            The page size will be changed so the rendered project can be fit on one page.|
|font_settings|Specifies font settings used when rendering project's view.|
|pages|Gets or sets a list of page numbers to save when saving project layout to separate files.|
|jpeg_quality|Gets or sets a JPEG quality. The allowed value range is 0..100.|
|reduce_footer_gap|Gets or sets a value indicating whether a gap between last task and the footer must be reduced.|
|tiff_compression|Gets or sets the type of compression to apply when saving generated images to the TIFF format.|
|pixel_format|Gets or sets the format of the color data for each pixel in the image.|
|horizontal_resolution|Gets or sets the horizontal resolution in dpi.|
|vertical_resolution|Gets or sets the vertical resolution in dpi.|
|page_saving_callback|Gets or sets a user-defined callback which is used to get an output stream for each rendered page.|

### See Also

* namespace [aspose.tasks.saving](/tasks/python-net/aspose.tasks.saving/)
* assembly [Aspose.Tasks](/tasks/python-net/)

