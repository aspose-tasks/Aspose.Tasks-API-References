---
title: Class PrimaveraSaveOptions
second_title: Aspose.Tasks for .NET API 参考
description: Aspose.Tasks.Saving.PrimaveraSaveOptions 班级. 允许在将项目保存为 Primavera XER 格式时指定其他选项
type: docs
weight: 1880
url: /zh/net/aspose.tasks.saving/primaverasaveoptions/
---
## PrimaveraSaveOptions class

允许在将项目保存为 Primavera XER 格式时指定其他选项。

```csharp
public class PrimaveraSaveOptions : SaveOptions
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [PrimaveraSaveOptions](primaverasaveoptions/)() | 初始化一个新的实例`PrimaveraSaveOptions`类. |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [ActivityIdIncrement](../../aspose.tasks.saving/primaverasaveoptions/activityidincrement/) { get; set; } | 获取或设置用于重新编号活动 ID 的增量。 |
| [ActivityIdPrefix](../../aspose.tasks.saving/primaverasaveoptions/activityidprefix/) { get; set; } | 获取或设置用于重新编号活动 ID 的前缀。 |
| [ActivityIdSuffix](../../aspose.tasks.saving/primaverasaveoptions/activityidsuffix/) { get; set; } | 获取或设置用于重新编号活动 ID 的后缀。 |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles/) { get; set; } | 获取或设置实例的列表[`BarStyle`](../../aspose.tasks.visualization/barstyle/)出现在项目视图中的类。 |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize/) { get; set; } | 获取或设置以磅为单位的自定义页面大小（1 磅 = 1/72 英寸）。 |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime/) { get; set; } | 获取或设置一个值，指示是否应绘制非工作时间（默认值为 TRUE）。 |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate/) { get; set; } | 获取或设置完成渲染的日期。 |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent/) { get; set; } | 获取或设置一个值，该值指示是否应增加行高以适合其内容。 |
| [FitTimescaleToEndOfPage](../../aspose.tasks.saving/saveoptions/fittimescaletoendofpage/) { get; set; } | 获取或设置视图的日历部分是否应呈现到最后一页的末尾（右侧）。 如果值为 false，日历部分将呈现到 EndDate，即使页面上有空白区域。 |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines/) { get; set; } | 获取或设置列表[`Gridline`](../../aspose.tasks.visualization/gridline/)出现在项目视图中. |
| [LegendOnEachPage](../../aspose.tasks.saving/saveoptions/legendoneachpage/) { get; set; } | 获取或设置一个值，指示是否应在每个页面上显示图例（默认值为 TRUE）。 |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks/) { get; set; } | 获取或设置一个值，指示关键任务是否应以红色显示（默认值为 FALSE）。 |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor/) { get; set; } | 获取或设置非工作时间颜色。 |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount/) { get; } | 获取或设置项目的页数。 |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize/) { get; set; } | 获取或设置要渲染的页面大小（默认值为PageSize.A4）。 |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | 获取或设置[`PresentationFormat`](../saveoptions/presentationformat/)文档将保存在其中。 |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage/) { get; set; } | 获取或设置一个值，该值指示当项目以图形格式保存时是否应将项目呈现到单个页面 。 页面大小将更改，以便呈现的项目适合一页。 |
| [RenumberActivityIds](../../aspose.tasks.saving/primaverasaveoptions/renumberactivityids/) { get; set; } | 获取或设置一个值，指示是否需要对活动 ID 重新编号。 |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars/) { get; set; } | 获取或设置一个值，指示是否应标记摘要任务栏上的子任务。 对于子任务，Rollup 字段指示是否将子任务甘特图栏上的信息汇总到摘要任务栏。 对于摘要任务，Rollup字段指示摘要任务栏是否显示汇总条。 您必须将摘要任务的汇总字段设置为是，以便任何子任务汇总到它们。 |
| [SaveFormat](../../aspose.tasks.saving/saveoptions/saveformat/) { get; } | 获取或设置如果使用此保存选项对象将保存文档的格式。 |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate/) { get; set; } | 获取或设置开始渲染的日期。 |
| [TasksComparer](../../aspose.tasks.saving/saveoptions/taskscomparer/) { get; set; } | 获取或设置比较器以对甘特图和任务表图表上的任务进行排序。 |
| [TasksFilter](../../aspose.tasks.saving/saveoptions/tasksfilter/) { get; set; } | 获取或设置用于过滤呈现在甘特图、任务表和任务使用情况图表上的任务的条件。 |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles/) { get; set; } | 获取或设置实例的列表[`TextStyle`](../../aspose.tasks.visualization/textstyle/)出现在项目视图中的类。 |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale/) { get; set; } | 获取或设置[`Timescale`](../saveoptions/timescale/)用于控制在项目保存为图形格式时如何呈现时间刻度（如果存在）的值。 |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush/) { get; set; } | 获取或设置一个值，该值指示在呈现甘特图时是否应使用渐变画笔。 |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | 获取或设置要呈现的视图列的列表（[`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/) ). 如果未设置，则仅呈现任务 ID、任务名称、开始和完成。 如果视图和[`ViewSettings`](../saveoptions/viewsettings/)属性已设置，View 中的列会覆盖 ViewSettings. 中的列 |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | 获取或设置视图（[`View`](../saveoptions/view/) ） 渲染。您可以使用此选项明确指定应将哪个视图保存为 PDF、HTML 或图像格式。 如果设置了此属性，[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/)保存项目时忽略属性。 视图应来自以下屏幕之一（（[`Screen`](../../aspose.tasks/view/screen/) )): (甘特图, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |

### 也可以看看

* class [SaveOptions](../saveoptions/)
* 命名空间 [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* 部件 [Aspose.Tasks](../../)


