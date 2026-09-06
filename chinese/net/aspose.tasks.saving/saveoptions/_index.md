---
title: "类 SaveOptions"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Saving.SaveOptions 类。这是一个抽象基类，用于允许用户在将项目保存为特定格式时指定其他选项的类。"
type: docs
weight: 2190
url: /zh/net/aspose.tasks.saving/saveoptions/
---
## SaveOptions class

这是一个抽象基类，供允许用户在将项目保存为特定格式时指定附加选项的类使用。

```csharp
public abstract class SaveOptions : SimpleSaveOptions
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles/) { get; set; } | 获取或设置出现在项目视图中的 [`BarStyle`](../../aspose.tasks.visualization/barstyle/) 类实例的列表。 |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize/) { get; set; } | 获取或设置自定义页面大小（单位为点，1 点 = 1/72 英寸）。 |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime/) { get; set; } | 获取或设置一个值，指示是否应绘制非工作时间（默认值为 TRUE）。 |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate/) { get; set; } | 获取或设置渲染结束的日期。 |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent/) { get; set; } | 获取或设置一个值，指示是否应增加行高以适应其内容。 |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines/) { get; set; } | 获取或设置出现在项目视图中的 [`Gridline`](../../aspose.tasks.visualization/gridline/) 列表。 |
| [IsPortrait](../../aspose.tasks.saving/saveoptions/isportrait/) { get; set; } | 获取或设置一个值，指示页面方向是否为纵向；如果页面方向为横向，则返回 false。 |
| [LegendDrawingOptions](../../aspose.tasks.saving/saveoptions/legenddrawingoptions/) { get; set; } | 获取或设置一个值，定义图例的渲染方式。默认值为 LegendDrawingOptions.OnEveryPage。 |
| [LegendItems](../../aspose.tasks.saving/saveoptions/legenditems/) { get; set; } | 获取或设置 PageLegendItem 数组，定义哪些条形应在页面图例中渲染。如果为 null，则渲染默认项。 |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks/) { get; set; } | 获取或设置一个值，指示关键任务是否应以红色显示（默认值为 FALSE）。 |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor/) { get; set; } | 获取或设置非工作时间的颜色。 |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount/) { get; } | 获取或设置项目的页数。 |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize/) { get; set; } | 获取或设置要渲染的页面大小（默认值为 PageSize.A4）。 |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | 获取或设置文档将保存的 [`PresentationFormat`](./presentationformat/)。 |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage/) { get; set; } | 获取或设置一个值，指示在项目以图形格式保存时是否应渲染为单页。页面大小将被更改，以便渲染的项目能够适配在一页上。 |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars/) { get; set; } | 获取或设置一个值，指示是否应在汇总任务条上标记子任务。对于子任务，Rollup 字段指示子任务甘特条的信息是否会汇总到汇总任务条。对于汇总任务，Rollup 字段指示汇总任务条是否显示已汇总的条形。必须将汇总任务的 Rollup 字段设置为 Yes，子任务才能汇总到它们上。 |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | 获取或设置如果使用此保存选项对象，文档将被保存的格式。 |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate/) { get; set; } | 获取或设置渲染开始的日期。 |
| [TaskLinkDrawingCallback](../../aspose.tasks.saving/saveoptions/tasklinkdrawingcallback/) { get; set; } | 获取或设置可用于自定义任务链接渲染某些方面的回调。 |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | 获取或设置用于在甘特图和任务表图上排序任务的比较器。 |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | 获取或设置用于过滤在甘特图、任务表和任务使用图上渲染的任务的条件。 |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles/) { get; set; } | 获取或设置在项目视图渲染期间应用的文本样式列表。 |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale/) { get; set; } | 获取或设置用于控制项目保存为图形格式时时间刻度（如果存在）呈现方式的 [`Timescale`](./timescale/) 值。 |
| [TimescaleFitBehavior](../../aspose.tasks.saving/saveoptions/timescalefitbehavior/) { get; set; } | 获取或设置定义如何将时间刻度的右端与页面末端对齐的行为。 |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush/) { get; set; } | 获取或设置指示在渲染甘特图时是否应使用渐变画刷的值。 |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | 获取或设置要呈现的视图列列表（[`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)）。如果未设置，则仅呈现任务 ID、任务名称、开始和结束。如果同时设置了 View 和 [`ViewSettings`](./viewsettings/) 属性，则 View 中的列会覆盖 ViewSettings 中的列。 |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | 获取或设置要呈现的视图（[`View`](./view/)）。您可以使用此选项显式指定应保存为 PDF、HTML 或图像格式的视图。如果设置了此属性，保存项目时将忽略 [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) 属性。视图应来自以下任一屏幕（[`Screen`](../../aspose.tasks/view/screen/)）：（Gantt、TaskSheet、TaskUsage、ResourceSheet、ResourceUsage）。 |

## 备注

将 SaveOptions 类的任何派生类实例传递给流 Save 或字符串 Save 重载，以便用户在保存文档时定义自定义选项。

## 示例

展示如何设置行高是否应增加以适应其内容的选项。

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    // 将“适应内容”选项设为 true
    FitContent = true,
    Timescale = Timescale.Months,
    PresentationFormat = PresentationFormat.TaskUsage
};
project.Save(OutDir + "FitContentsToCellSize_out.pdf", options);
```

### 另见

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


