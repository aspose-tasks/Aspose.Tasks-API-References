---
title: "Aspose::Tasks::Saving::SaveOptions class"
linktitle: "SaveOptions"
articleTitle: "SaveOptions"
second_title: "Aspose.Tasks for C++"
description: "This is an abstract base class for classes that allow the user to specify additional options when saving a project into a particular format."
type: docs
weight: 10
url: /cpp/aspose.tasks.saving/saveoptions/
---

## SaveOptions class

**Inherits:** Aspose::Tasks::Saving::SimpleSaveOptions

This is an abstract base class for classes that allow the user to specify additional options when saving a project into a particular format.

An instance of any derived class from SaveOptions class is passed to the stream Save or string Save overloads for the user to define custom options when saving a document.

## Methods

| Name | Description |
| --- | --- |
| [get_BarStyles](./get_barstyles/) | Gets the list of the instances of the BarStyle class that appear in project view. |
| [get_CustomPageSize](./get_custompagesize/) | Gets the custom page size in points (1 point = 1/72 of inch). |
| [get_DrawNonWorkingTime](./get_drawnonworkingtime/) | Gets a value indicating whether non-working time should be drawn (Default value is TRUE). |
| [get_EndDate](./get_enddate/) | Gets a date to finish rendering to. |
| [get_FitContent](./get_fitcontent/) | Gets a value indicating whether row height should be increased to fit its content. |
| [get_FitTimescaleToEndOfPage](./get_fittimescaletoendofpage/) | Gets whether a calendar section of a view should be rendered to the end (right side) of the last page. If value is false, calendar section is rendered exactly to EndDate, even there is an empty space on a page. |
| [get_Gridlines](./get_gridlines/) | Gets a list of Gridline that appear in project view. |
| [get_IsPortrait](./get_isportrait/) | Gets a value indicating whether the page orientation is portrait; returns false if the page orientation is landscape. |
| [get_LegendDrawingOptions](./get_legenddrawingoptions/) | Gets a value which define how to render a legend. Default value is LegendDrawingOptions.OnEveryPage. |
| [get_LegendItems](./get_legenditems/) | Gets an array of PageLegendItem which define which bars should be rendered in page legend. If null, the default items are rendered. |
| [get_MarkCriticalTasks](./get_markcriticaltasks/) | Gets a value indicating whether critical tasks should be displayed in red color (Default value is FALSE). |
| [get_NonWorkingTimeColor](./get_nonworkingtimecolor/) | Gets the non-working time color. |
| [get_PageCount](./get_pagecount/) | Gets the number of pages of project. |
| [get_PageSize](./get_pagesize/) | Gets the size of page to be rendered (Default value is PageSize.A4). |
| [get_PresentationFormat](./get_presentationformat/) | Gets the PresentationFormat in which the document will be saved. |
| [get_RenderToSinglePage](./get_rendertosinglepage/) | Gets a value indicating whether a project should be rendered to a single page when project is saved in graphical format. The page size will be changed so the rendered project can be fit on one page. |
| [get_RollUpGanttBars](./get_rollupganttbars/) | Gets a value indicating whether subtasks on the summary task bar should be marked. For subtasks, the Rollup field indicates whether information on the subtask Gantt bars will be rolled up to the summary task bar. For summary tasks, the Rollup field indicates whether the summary task bar displays rolled up bars. You must have the Rollup field for summary tasks set to Yes for any subtasks to roll up to them. |
| [get_StartDate](./get_startdate/) | Gets the date to start rendering from. |
| [get_TextStyles](./get_textstyles/) | Gets the list of text styles that applied during rendering of a project view. |
| [get_Timescale](./get_timescale/) | Gets the Timescale value which is used to control how timescale (if present) is rendered when project is saved to graphical format. |
| [get_TimescaleFitBehavior](./get_timescalefitbehavior/) | Gets a behavior which define how to align right end of the timescale with the page end. |
| [get_UseGradientBrush](./get_usegradientbrush/) | Gets a value indicating whether gradient brush should be used when rendering Gantt Chart. |
| [get_View](./get_view/) | Gets a list of the view columns to render ( GanttChartColumn ). If not set then task ids, task names, start and finish are rendered only. If both View and ViewSettings properties are set, columns from View overrides columns from ViewSettings. |
| [get_ViewSettings](./get_viewsettings/) | Gets a view ( View ) to render. You can use this options to explicitly specify which view should be saved to PDF, HTML or Image formats. If this property is set, Visualization::PresentationFormat property is ignored when project is saved. View should be from one of the following screen (( Aspose::Tasks::View::Screen )): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |
| [set_BarStyles](./set_barstyles/) | Sets the list of the instances of the BarStyle class that appear in project view. |
| [set_CustomPageSize](./set_custompagesize/) | Sets the custom page size in points (1 point = 1/72 of inch). |
| [set_DrawNonWorkingTime](./set_drawnonworkingtime/) | Sets a value indicating whether non-working time should be drawn (Default value is TRUE). |
| [set_EndDate](./set_enddate/) | Sets a date to finish rendering to. |
| [set_FitContent](./set_fitcontent/) | Sets a value indicating whether row height should be increased to fit its content. |
| [set_FitTimescaleToEndOfPage](./set_fittimescaletoendofpage/) | Sets whether a calendar section of a view should be rendered to the end (right side) of the last page. If value is false, calendar section is rendered exactly to EndDate, even there is an empty space on a page. |
| [set_Gridlines](./set_gridlines/) | Sets a list of Gridline that appear in project view. |
| [set_IsPortrait](./set_isportrait/) | Sets a value indicating whether the page orientation is portrait; returns false if the page orientation is landscape. |
| [set_LegendDrawingOptions](./set_legenddrawingoptions/) | Sets a value which define how to render a legend. Default value is LegendDrawingOptions.OnEveryPage. |
| [set_LegendItems](./set_legenditems/) | Sets an array of PageLegendItem which define which bars should be rendered in page legend. If null, the default items are rendered. |
| [set_MarkCriticalTasks](./set_markcriticaltasks/) | Sets a value indicating whether critical tasks should be displayed in red color (Default value is FALSE). |
| [set_NonWorkingTimeColor](./set_nonworkingtimecolor/) | Sets the non-working time color. |
| [set_PageSize](./set_pagesize/) | Sets the size of page to be rendered (Default value is PageSize.A4). |
| [set_PresentationFormat](./set_presentationformat/) | Sets the PresentationFormat in which the document will be saved. |
| [set_RenderToSinglePage](./set_rendertosinglepage/) | Sets a value indicating whether a project should be rendered to a single page when project is saved in graphical format. The page size will be changed so the rendered project can be fit on one page. |
| [set_RollUpGanttBars](./set_rollupganttbars/) | Sets a value indicating whether subtasks on the summary task bar should be marked. For subtasks, the Rollup field indicates whether information on the subtask Gantt bars will be rolled up to the summary task bar. For summary tasks, the Rollup field indicates whether the summary task bar displays rolled up bars. You must have the Rollup field for summary tasks set to Yes for any subtasks to roll up to them. |
| [set_StartDate](./set_startdate/) | Sets the date to start rendering from. |
| [set_TextStyles](./set_textstyles/) | Sets the list of text styles that applied during rendering of a project view. |
| [set_Timescale](./set_timescale/) | Sets the Timescale value which is used to control how timescale (if present) is rendered when project is saved to graphical format. |
| [set_TimescaleFitBehavior](./set_timescalefitbehavior/) | Sets a behavior which define how to align right end of the timescale with the page end. |
| [set_UseGradientBrush](./set_usegradientbrush/) | Sets a value indicating whether gradient brush should be used when rendering Gantt Chart. |
| [set_View](./set_view/) | Sets a list of the view columns to render ( GanttChartColumn ). If not set then task ids, task names, start and finish are rendered only. If both View and ViewSettings properties are set, columns from View overrides columns from ViewSettings. |
| [set_ViewSettings](./set_viewsettings/) | Sets a view ( View ) to render. You can use this options to explicitly specify which view should be saved to PDF, HTML or Image formats. If this property is set, Visualization::PresentationFormat property is ignored when project is saved. View should be from one of the following screen (( Aspose::Tasks::View::Screen )): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |

