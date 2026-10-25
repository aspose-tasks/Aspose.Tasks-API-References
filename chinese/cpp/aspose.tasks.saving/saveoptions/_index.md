---
title: "Aspose::Tasks::Saving::SaveOptions class"
linktitle: "SaveOptions"
articleTitle: "SaveOptions"
second_title: "Aspose.Tasks for C++"
description: "这是一个抽象基类，用于允许用户在将项目保存为特定格式时指定附加选项的类。"
type: docs
weight: 10
url: /zh/cpp/aspose.tasks.saving/saveoptions/
---

## SaveOptions class

**Inherits:** Aspose::Tasks::Saving::SimpleSaveOptions

这是一个抽象基类，用于允许用户在将项目保存为特定格式时指定附加选项的类。

任何从 SaveOptions 类派生的类的实例都会传递给流 Save 或字符串 Save 重载，以便用户在保存文档时定义自定义选项。

## 方法

| 表示 ResourceAssignment 对象的属性。 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| [get_BarStyles](./get_barstyles/) | 获取出现在项目视图中的 BarStyle 类实例列表。 |
| [get_CustomPageSize](./get_custompagesize/) | 获取以点为单位的自定义页面大小（1 点 = 1/72 英寸）。 |
| [get_DrawNonWorkingTime](./get_drawnonworkingtime/) | 获取一个值，指示是否应绘制非工作时间（默认值为 TRUE）。 |
| [get_EndDate](./get_enddate/) | 获取用于结束渲染的日期。 |
| [get_FitContent](./get_fitcontent/) | 获取一个值，指示是否应增加行高以适应其内容。 |
| [get_FitTimescaleToEndOfPage](./get_fittimescaletoendofpage/) | 获取视图的日历部分是否应渲染到最后一页的末端（右侧）。如果值为 false，日历部分将精确渲染到 EndDate，即使页面上有空白空间。 |
| [get_Gridlines](./get_gridlines/) | 获取出现在项目视图中的 Gridline 列表。 |
| [get_IsPortrait](./get_isportrait/) | 获取一个值，指示页面方向是否为纵向；如果页面方向为横向，则返回 false。 |
| [get_LegendDrawingOptions](./get_legenddrawingoptions/) | 获取定义图例渲染方式的值。默认值为 LegendDrawingOptions.OnEveryPage。 |
| [get_LegendItems](./get_legenditems/) | 获取一个 PageLegendItem 数组，用于定义哪些条形应在页面图例中渲染。如果为 null，则渲染默认项。 |
| [get_MarkCriticalTasks](./get_markcriticaltasks/) | 获取一个值，指示关键任务是否应以红色显示（默认值为 FALSE）。 |
| [get_NonWorkingTimeColor](./get_nonworkingtimecolor/) | 获取非工作时间的颜色。 |
| [get_PageCount](./get_pagecount/) | 获取项目的页数。 |
| [get_PageSize](./get_pagesize/) | 获取要渲染的页面大小（默认值为 PageSize.A4）。 |
| [get_PresentationFormat](./get_presentationformat/) | 获取文档将被保存的 PresentationFormat。 |
| [get_RenderToSinglePage](./get_rendertosinglepage/) | 获取一个值，指示在以图形格式保存项目时是否应将项目渲染为单页。页面大小将被调整，以便渲染的项目能够适配在一页上。 |
| [get_RollUpGanttBars](./get_rollupganttbars/) | 获取一个值，指示是否应标记汇总任务栏上的子任务。对于子任务，Rollup 字段指示子任务甘特条的信息是否会汇总到汇总任务栏。对于汇总任务，Rollup 字段指示汇总任务栏是否显示已汇总的条形。必须将汇总任务的 Rollup 字段设置为 Yes，子任务才能汇总到其上。 |
| [get_StartDate](./get_startdate/) | 获取渲染的起始日期。 |
| [get_TextStyles](./get_textstyles/) | 获取在项目视图渲染期间应用的文本样式列表。 |
| [get_Timescale](./get_timescale/) | 获取用于控制在将项目保存为图形格式时时间刻度（如果存在）如何渲染的 Timescale 值。 |
| [get_TimescaleFitBehavior](./get_timescalefitbehavior/) | 获取定义如何将时间刻度的右端与页面末端对齐的行为。 |
| [get_UseGradientBrush](./get_usegradientbrush/) | 获取一个值，指示在渲染甘特图时是否应使用渐变画刷。 |
| [get_View](./get_view/) | 获取要渲染的视图列列表（ GanttChartColumn ）。如果未设置，则仅渲染任务 ID、任务名称、开始和结束。如果同时设置了 View 和 ViewSettings 属性，则 View 的列会覆盖 ViewSettings 的列。 |
| [get_ViewSettings](./get_viewsettings/) | 获取要渲染的视图（ View ）。您可以使用此选项显式指定应保存为 PDF、HTML 或 Image 格式的视图。如果设置了此属性，保存项目时会忽略 Visualization::PresentationFormat 属性。View 应来自以下屏幕之一 (( Aspose::Tasks::View::Screen ))：（Gantt、TaskSheet、TaskUsage、ResourceSheet、ResourceUsage） |
| [set_BarStyles](./set_barstyles/) | 设置出现在项目视图中的 BarStyle 类实例列表。 |
| [set_CustomPageSize](./set_custompagesize/) | 设置自定义页面大小，单位为点（1 点 = 1/72 英寸）。 |
| [set_DrawNonWorkingTime](./set_drawnonworkingtime/) | 设置一个值，指示是否应绘制非工作时间（默认值为 TRUE）。 |
| [set_EndDate](./set_enddate/) | 设置渲染结束的日期。 |
| [set_FitContent](./set_fitcontent/) | 设置一个值，指示是否应增加行高以适应其内容。 |
| [set_FitTimescaleToEndOfPage](./set_fittimescaletoendofpage/) | 设置视图的日历部分是否应渲染到最后一页的末端（右侧）。如果值为 false，日历部分将精确渲染到 EndDate，即使页面上有空白空间。 |
| [set_Gridlines](./set_gridlines/) | 设置出现在项目视图中的 Gridline 列表。 |
| [set_IsPortrait](./set_isportrait/) | 设置一个值，指示页面方向是否为纵向；如果页面方向为横向则返回 false。 |
| [set_LegendDrawingOptions](./set_legenddrawingoptions/) | 设置一个值，定义如何渲染图例。默认值为 LegendDrawingOptions.OnEveryPage。 |
| [set_LegendItems](./set_legenditems/) | 设置一个 PageLegendItem 数组，定义哪些条形应在页面图例中渲染。如果为 null，则渲染默认项。 |
| [set_MarkCriticalTasks](./set_markcriticaltasks/) | 设置一个值，指示关键任务是否应以红色显示（默认值为 FALSE）。 |
| [set_NonWorkingTimeColor](./set_nonworkingtimecolor/) | 设置非工作时间的颜色。 |
| [set_PageSize](./set_pagesize/) | 设置要渲染的页面大小（默认值为 PageSize.A4）。 |
| [set_PresentationFormat](./set_presentationformat/) | 设置文档将被保存的 PresentationFormat。 |
| [set_RenderToSinglePage](./set_rendertosinglepage/) | 设置一个值，指示在项目以图形格式保存时是否应渲染为单页。页面大小将被调整，以便渲染的项目能够适应一页。 |
| [set_RollUpGanttBars](./set_rollupganttbars/) | 设置一个值，指示是否应在汇总任务条上标记子任务。对于子任务，Rollup 字段指示子任务甘特条的信息是否会汇总到汇总任务条。对于汇总任务，Rollup 字段指示汇总任务条是否显示已汇总的条形。必须将汇总任务的 Rollup 字段设置为 Yes，子任务才能汇总到其上。 |
| [set_StartDate](./set_startdate/) | 设置渲染的起始日期。 |
| [set_TextStyles](./set_textstyles/) | 设置在项目视图渲染期间应用的文本样式列表。 |
| [set_Timescale](./set_timescale/) | 设置 Timescale 值，用于控制在项目保存为图形格式时如何渲染时间刻度（如果存在）。 |
| [set_TimescaleFitBehavior](./set_timescalefitbehavior/) | 设置一种行为，定义如何将时间刻度的右端与页面末端对齐。 |
| [set_UseGradientBrush](./set_usegradientbrush/) | 设置一个值，指示在渲染甘特图时是否应使用渐变画刷。 |
| [set_View](./set_view/) | 设置要渲染的视图列列表（ GanttChartColumn ）。如果未设置，则仅渲染任务 ID、任务名称、开始和结束。如果同时设置了 View 和 ViewSettings 属性，则 View 的列会覆盖 ViewSettings 的列。 |
| [set_ViewSettings](./set_viewsettings/) | 设置要渲染的视图（ View ）。您可以使用此选项显式指定应保存为 PDF、HTML 或 Image 格式的视图。如果设置了此属性，保存项目时会忽略 Visualization::PresentationFormat 属性。View 应来自以下屏幕之一 (( Aspose::Tasks::View::Screen ))：（Gantt、TaskSheet、TaskUsage、ResourceSheet、ResourceUsage） |

