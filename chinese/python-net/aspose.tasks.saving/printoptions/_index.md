---
title: "PrintOptions"
second_title: "适用于 Python via .NET 的 Aspose.Tasks API 参考"
description: 
type: docs
weight: 120
url: /zh/python-net/aspose.tasks.saving/printoptions/
---

## PrintOptions class

允许在打印项目时指定其他选项。

PrintOptions 类型公开以下成员：
## 构造函数
| 名称 | 描述 |
| :- | :- |
| PrintOptions() | 初始化一个新的 [PrintOptions](/tasks/python-net/aspose.tasks.saving/printoptions/) 类实例，可用于设置打印项目的不同选项。 |
## 属性
| 名称 | 描述 |
| :- | :- |
| save_format |  |
| bar_styles | 获取或设置在项目视图中出现的 [BarStyle](/tasks/python-net/aspose.tasks.visualization/barstyle/) 类实例的列表。 |
| draw_non_working_time | 获取或设置一个值，指示是否应绘制非工作时间（默认值为 TRUE）。 |
| end_date | 获取或设置渲染结束的日期。 |
| timescale_fit_behavior | 获取或设置一种行为，定义如何将时间刻度的右端与页面末端对齐。 |
| fit_content | 获取或设置一个值，指示是否应增加行高以适应其内容。 |
| gridlines | 获取或设置在项目视图中出现的 [Gridline](/tasks/python-net/aspose.tasks.visualization/gridline/) 列表。 |
| legend_drawing_options | 获取或设置定义如何渲染图例的值。默认值为 LegendDrawingOptions.OnEveryPage。 |
| legend_items | 获取或设置一个 PageLegendItem 数组，用于定义应在页面图例中渲染哪些条形。<br/>            如果为 null，则渲染默认项。 |
| mark_critical_tasks | 获取或设置指示是否应以红色显示关键任务的值（默认值为 FALSE）。 |
| non_working_time_color | 获取或设置非工作时间的颜色。 |
| page_count | 获取或设置项目的页数。 |
| page_size | 获取或设置要渲染的页面大小（默认值为 PageSize.A4）。 |
| is_portrait | 获取或设置指示页面方向是否为纵向的值；如果页面方向为横向，则返回 false。 |
| presentation_format | 获取或设置文档将被保存的 [presentation_format](/tasks/python-net/aspose.tasks.saving/saveoptions/)。 |
| roll_up_gantt_bars | 获取或设置指示是否应标记汇总任务栏上的子任务的值。<br/>            对于子任务，Rollup 字段指示子任务甘特条的信息是否会汇总到汇总任务栏。<br/>            对于汇总任务，Rollup 字段指示汇总任务栏是否显示已汇总的条形。<br/>            必须将汇总任务的 Rollup 字段设置为 Yes，子任务才能汇总到它们。 |
| start_date | 获取或设置开始渲染的日期。 |
| text_styles | 获取或设置在项目视图渲染期间应用的文本样式列表。 |
| timescale | 获取或设置用于控制项目保存为图形格式时时间刻度（如果存在）如何渲染的 [timescale](/tasks/python-net/aspose.tasks.saving/saveoptions/) 值。 |
| use_gradient_brush | 获取或设置一个值，指示在渲染甘特图时是否应使用渐变画笔。 |
| view | 获取或设置要渲染的视图列列表 ([GanttChartColumn](/tasks/python-net/aspose.tasks.visualization/ganttchartcolumn/))。<br/>            如果未设置，则仅渲染任务 ID、任务名称、开始和结束。<br/>            如果同时设置了 View 和 [view_settings](/tasks/python-net/aspose.tasks.saving/saveoptions/) 属性，则 View 中的列会覆盖 ViewSettings 中的列。 |
| view_settings | 获取或设置要渲染的视图 ([view](/tasks/python-net/aspose.tasks.saving/saveoptions/))。您可以使用此选项明确指定应保存为 PDF、HTML 或图像格式的视图。<br/>            如果设置了此属性，保存项目时将忽略 [PresentationFormat](/tasks/python-net/aspose.tasks.visualization/presentationformat/) 属性。<br/>            视图应来自以下屏幕之一 (([screen](/tasks/python-net/aspose.tasks/view/)))： (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |
| custom_page_size | 获取或设置以点为单位的自定义页面大小（1 点 = 1/72 英寸）。 |
| render_to_single_page | 获取或设置一个值，指示项目在保存为图形格式时是否应渲染为单页<br/>            当项目以图形格式保存时。<br/>            页面大小将被更改，以便渲染的项目能够适应一页。 |

### 另见

* namespace [aspose.tasks.saving](/tasks/python-net/aspose.tasks.saving/)
* assembly [Aspose.Tasks](/tasks/python-net/)

