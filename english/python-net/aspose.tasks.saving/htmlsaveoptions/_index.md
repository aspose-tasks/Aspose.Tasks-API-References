---
title: HtmlSaveOptions
second_title: Aspose.Tasks for Python via .NET API Reference
description: 
type: docs
weight: 20
url: /python-net/aspose.tasks.saving/htmlsaveoptions/
---

## HtmlSaveOptions class

Allows to specify additional options when rendering project pages to HTML.

The HtmlSaveOptions type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|HtmlSaveOptions()|Initializes a new instance of the [HtmlSaveOptions](/tasks/python-net/aspose.tasks.saving/htmlsaveoptions/) class.|
## Properties
| Name | Description |
| :- | :- |
|save_format|  |
|bar_styles|Gets or sets the list of the instances of the [BarStyle](/tasks/python-net/aspose.tasks.visualization/barstyle/) class that appear in project view.|
|draw_non_working_time|Gets or sets a value indicating whether non-working time should be drawn (Default value is TRUE).|
|end_date|Gets or sets a date to finish rendering to.|
|fit_timescale_to_end_of_page|Gets or sets whether a calendar section of a view should be rendered to the end (right side) of the last page.<br/>            If value is false, calendar section is rendered exactly to EndDate, even there is an empty space on a page.|
|timescale_fit_behavior|Gets or sets a behavior which define how to align right end of the timescale with the page end.|
|fit_content|Gets or sets a value indicating whether row height should be increased to fit its content.|
|gridlines|Gets or sets a list of [Gridline](/tasks/python-net/aspose.tasks.visualization/gridline/) that appear in project view.|
|legend_drawing_options|Gets or sets a value which define how to render a legend. Default value is LegendDrawingOptions.OnEveryPage.|
|legend_items|Gets or sets an array of PageLegendItem which define which bars should be rendered in page legend.<br/>            If null, the default items are rendered.|
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
|use_gradient_brush|Gets or sets a value indicating whether to use gradient brush when rendering project layout.|
|view|Gets or sets a list of the view columns to render ([GanttChartColumn](/tasks/python-net/aspose.tasks.visualization/ganttchartcolumn/)).<br/>            If not set then task ids, task names, start and finish are rendered only.<br/>            If both View and [view_settings](/tasks/python-net/aspose.tasks.saving/saveoptions/) properties are set, columns from View overrides columns from ViewSettings.|
|view_settings|Gets or sets a view ([view](/tasks/python-net/aspose.tasks.saving/saveoptions/)) to render. You can use this options to explicitly specify which view should be saved to PDF, HTML or Image formats.<br/>            If this property is set, [PresentationFormat](/tasks/python-net/aspose.tasks.visualization/presentationformat/) property is ignored when project is saved.<br/>            View should be from one of the following screen (([screen](/tasks/python-net/aspose.tasks/view/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage)|
|custom_page_size|Gets or sets the custom page size in points (1 point = 1/72 of inch).|
|render_to_single_page|Gets or sets a value indicating whether a project should be rendered to a single page<br/>            when project is saved in graphical format.<br/>            The page size will be changed so the rendered project can be fit on one page.|
|css_style_prefix|Gets or sets CSS style prefix.|
|font_settings|Specifies font settings used when rendering project's view.|
|reduce_footer_gap|Gets or sets a value indicating whether a gap between last task and the footer must be reduced.|
|include_project_name_in_page_header|Gets or sets a value indicating whether to include project name in HTML page header.|
|include_project_name_in_title|Gets or sets a value indicating whether to include project name in HTML title.|
|pages|Gets or sets a list of page numbers to save when rendering project layout.|
|export_css|Gets or sets the way CSS are exported.|
|export_images|Gets or sets the way images are exported.|
|export_fonts|Gets or sets the way fonts are exported.|
|css_saving_callback|Gets or sets the callback that is called to create resource to store CSS.|
|font_saving_callback|Gets or sets the callback that is called to create resource to store font.|
|image_saving_callback|Gets or sets the callback that is called to create resource to store font.|
|font_face_types|Gets or sets the font face types.|
|page_saving_callback|Gets or sets a user-defined callback which is used to get an output stream for each rendered page.|

### See Also

* namespace [aspose.tasks.saving](/tasks/python-net/aspose.tasks.saving/)
* assembly [Aspose.Tasks](/tasks/python-net/)

