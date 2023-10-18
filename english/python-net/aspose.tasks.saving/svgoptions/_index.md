---
title: SvgOptions
second_title: Aspose.Tasks for Python via .NET API Reference
description: 
type: docs
weight: 170
url: /python-net/aspose.tasks.saving/svgoptions/
---

## SvgOptions class

Allows to specify additional options when rendering project pages to SVG.

The SvgOptions type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|SvgOptions()|Initializes a new instance of the|
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
|mark_critical_tasks|Gets or sets a value indicating whether critical tasks should be displayed in red color (Default value is FALSE).|
|non_working_time_color|Gets or sets the non-working time color.|
|page_count|Gets or sets the number of pages of project.|
|page_size|Gets or sets the size of page to be rendered (Default value is PageSize.A4).|
|presentation_format|Gets or sets the|
|roll_up_gantt_bars|Gets or sets a value indicating whether subtasks on the summary task bar should be marked.<br/>            For subtasks, the Rollup field indicates whether information on the subtask Gantt bars will be rolled up to the summary task bar.<br/>            For summary tasks, the Rollup field indicates whether the summary task bar displays rolled up bars.<br/>            You must have the Rollup field for summary tasks set to Yes for any subtasks to roll up to them.|
|start_date|Gets or sets the date to start rendering from.|
|text_styles|Gets or sets the list of the instances of the|
|timescale|Gets or sets the|
|use_gradient_brush|Determines whether to use gradient brush when rendering project layout.|
|view|Gets or sets a list of the view columns to render (|
|view_settings|Gets or sets a view (|
|custom_page_size|Gets or sets the custom page size in points (1 point = 1/72 of inch).|
|render_to_single_page|Gets or sets a value indicating whether a project should be rendered to a single page<br/>            when project is saved in graphical format.<br/>            The page size will be changed so the rendered project can be fit on one page.|
|page_saving_callback|Gets or sets a user-defined implementation callback which is used to get an output stream for each rendered page.|

### See Also

* namespace [aspose.tasks.saving](/tasks/python-net/aspose.tasks.saving/)
* assembly [Aspose.Tasks](/tasks/python-net/)

