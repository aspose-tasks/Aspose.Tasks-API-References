---
title: PdfSaveOptions
second_title: Aspose.Tasks for Python via .NET API Reference
description: 
type: docs
weight: 90
url: /python-net/aspose.tasks.saving/pdfsaveoptions/
---

## PdfSaveOptions class

Allows to specify additional options when rendering project pages to PDF.

The PdfSaveOptions type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|PdfSaveOptions()|Initializes a new instance of the|
## Properties
| Name | Description |
| :- | :- |
|save_format|  |
|bar_styles|Gets or sets the list of the instances of the|
|draw_non_working_time|Gets or sets a value indicating whether non-working time should be drawn (Default value is TRUE).|
|end_date|Gets or sets a date to finish rendering to.|
|fit_timescale_to_end_of_page|Gets or sets whether a calendar section of a view should be rendered to the end (right side) of the last page.<br/>            If value is false, calendar section is rendered exactly to EndDate, even there is an empty space on a page.|
|fit_content|Gets or sets a value indicating whether row height should be increased to fit its content.|
|gridlines|Gets or sets a list of|
|legend_on_each_page|Gets or sets a value indicating whether legend should be shown on each page (Default value is TRUE).|
|legend_drawing_options|Gets or sets a value which define how to render a legend. Default value is LegendDrawingOptions.OnEveryPage.|
|mark_critical_tasks|Gets or sets a value indicating whether critical tasks should be displayed in red color (Default value is FALSE).|
|non_working_time_color|Gets or sets the non-working time color.|
|page_count|Gets or sets the number of pages of project.|
|page_size|Gets or sets the size of page to be rendered (Default value is PageSize.A4).|
|is_portrait|Gets or sets a value indicating whether the page orientation is portrait; returns false if the page orientation is landscape.|
|presentation_format|Gets or sets the|
|roll_up_gantt_bars|Gets or sets a value indicating whether subtasks on the summary task bar should be marked.<br/>            For subtasks, the Rollup field indicates whether information on the subtask Gantt bars will be rolled up to the summary task bar.<br/>            For summary tasks, the Rollup field indicates whether the summary task bar displays rolled up bars.<br/>            You must have the Rollup field for summary tasks set to Yes for any subtasks to roll up to them.|
|start_date|Gets or sets the date to start rendering from.|
|text_styles|Gets or sets the list of the instances of the|
|timescale|Gets or sets the|
|use_gradient_brush|Gets or sets a value indicating whether gradient brush should be used when rendering Gantt Chart.|
|view|Gets or sets a list of the view columns to render (|
|view_settings|Gets or sets a view (|
|custom_page_size|Gets or sets the custom page size in points (1 point = 1/72 of inch).|
|render_to_single_page|Gets or sets a value indicating whether a project should be rendered to a single page<br/>            when project is saved in graphical format.<br/>            The page size will be changed so the rendered project can be fit on one page.|
|reduce_footer_gap|Gets or sets a value indicating whether a gap between last task and the footer must be reduced.|
|compliance|Gets or sets a desired compliance level for generated PDF document.<br/>            Default is|
|encryption_details|Gets or sets a encryption details. If not set, then no encryption will be performed.|
|text_compression|Gets or sets a compression type to be used for all content streams except images.<br/>            Default is|
|digital_signature_details|Gets or sets a digital signature details. If not set, then no signing will be performed.|
|save_to_separate_files|Gets or sets a value indicating whether to save project pages to separate files.|
|page_saving_callback|Gets or sets a user-defined callback which is used to get an output stream for each rendered page.<br/>            Is applicable when|
|pages|Gets or sets the list of pages numbers to save when saving project layout to separate files.|
|font_settings|Specifies font settings used when rendering project's view.|

### See Also

* namespace [aspose.tasks.saving](/tasks/python-net/aspose.tasks.saving/)
* assembly [Aspose.Tasks](/tasks/python-net/)

