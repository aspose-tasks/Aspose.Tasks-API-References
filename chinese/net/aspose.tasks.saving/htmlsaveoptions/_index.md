---
title: "类 HtmlSaveOptions"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Saving.HtmlSaveOptions 类。允许在将项目页面渲染为 HTML 时指定其他选项"
type: docs
weight: 2010
url: /zh/net/aspose.tasks.saving/htmlsaveoptions/
---
## HtmlSaveOptions class

允许在将项目页面渲染为 HTML 时指定附加选项。

```csharp
public class HtmlSaveOptions : SaveOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions/)() | 初始化 `HtmlSaveOptions` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles/) { get; set; } | 获取或设置出现在项目视图中的 [`BarStyle`](../../aspose.tasks.visualization/barstyle/) 类实例的列表。 |
| [CssSavingCallback](../../aspose.tasks.saving/htmlsaveoptions/csssavingcallback/) { get; set; } | 获取或设置用于创建存储 CSS 的资源的回调函数。 |
| [CssStylePrefix](../../aspose.tasks.saving/htmlsaveoptions/cssstyleprefix/) { get; set; } | 获取或设置 CSS 样式前缀。 |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize/) { get; set; } | 获取或设置自定义页面大小（单位为点，1 点 = 1/72 英寸）。 |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime/) { get; set; } | 获取或设置一个值，指示是否应绘制非工作时间（默认值为 TRUE）。 |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate/) { get; set; } | 获取或设置渲染结束的日期。 |
| [ExportCss](../../aspose.tasks.saving/htmlsaveoptions/exportcss/) { get; set; } | 获取或设置 CSS 的导出方式。 |
| [ExportFonts](../../aspose.tasks.saving/htmlsaveoptions/exportfonts/) { get; set; } | 获取或设置字体的导出方式。 |
| [ExportImages](../../aspose.tasks.saving/htmlsaveoptions/exportimages/) { get; set; } | 获取或设置图像的导出方式。 |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent/) { get; set; } | 获取或设置一个值，指示是否应增加行高以适应其内容。 |
| [FontFaceTypes](../../aspose.tasks.saving/htmlsaveoptions/fontfacetypes/) { get; set; } | 获取或设置字体族类型。 |
| [FontSavingCallback](../../aspose.tasks.saving/htmlsaveoptions/fontsavingcallback/) { get; set; } | 获取或设置用于创建存储字体资源的回调。 |
| [FontSettings](../../aspose.tasks.saving/htmlsaveoptions/fontsettings/) { get; } | 指定在渲染项目视图时使用的字体设置。 |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines/) { get; set; } | 获取或设置出现在项目视图中的 [`Gridline`](../../aspose.tasks.visualization/gridline/) 列表。 |
| [ImageSavingCallback](../../aspose.tasks.saving/htmlsaveoptions/imagesavingcallback/) { get; set; } | 获取或设置用于创建存储字体资源的回调。 |
| [IncludeProjectNameInPageHeader](../../aspose.tasks.saving/htmlsaveoptions/includeprojectnameinpageheader/) { get; set; } | 获取或设置一个值，指示是否在 HTML 页面标题中包含项目名称。 |
| [IncludeProjectNameInTitle](../../aspose.tasks.saving/htmlsaveoptions/includeprojectnameintitle/) { get; set; } | 获取或设置一个值，指示是否在 HTML 标题中包含项目名称。 |
| [IsPortrait](../../aspose.tasks.saving/saveoptions/isportrait/) { get; set; } | 获取或设置一个值，指示页面方向是否为纵向；如果页面方向为横向，则返回 false。 |
| [LegendDrawingOptions](../../aspose.tasks.saving/saveoptions/legenddrawingoptions/) { get; set; } | 获取或设置一个值，定义图例的渲染方式。默认值为 LegendDrawingOptions.OnEveryPage。 |
| [LegendItems](../../aspose.tasks.saving/saveoptions/legenditems/) { get; set; } | 获取或设置 PageLegendItem 数组，定义哪些条形应在页面图例中渲染。如果为 null，则渲染默认项。 |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks/) { get; set; } | 获取或设置一个值，指示关键任务是否应以红色显示（默认值为 FALSE）。 |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor/) { get; set; } | 获取或设置非工作时间的颜色。 |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount/) { get; } | 获取或设置项目的页数。 |
| [Pages](../../aspose.tasks.saving/htmlsaveoptions/pages/) { get; set; } | 获取或设置在渲染项目布局时要保存的页码列表。如果此列表为空，将保存所有项目页面。 |
| [PageSavingCallback](../../aspose.tasks.saving/htmlsaveoptions/pagesavingcallback/) { get; set; } | 获取或设置用户定义的回调，用于获取每个渲染页面的输出流。 |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize/) { get; set; } | 获取或设置要渲染的页面大小（默认值为 PageSize.A4）。 |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | 获取或设置文档将保存的 [`PresentationFormat`](../saveoptions/presentationformat/)。 |
| [ReduceFooterGap](../../aspose.tasks.saving/htmlsaveoptions/reducefootergap/) { get; set; } | 获取或设置一个值，指示是否必须缩小最后任务与页脚之间的间距。 |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage/) { get; set; } | 获取或设置一个值，指示在项目以图形格式保存时是否应渲染为单页。页面大小将被更改，以便渲染的项目能够适配在一页上。 |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars/) { get; set; } | 获取或设置一个值，指示是否应在汇总任务条上标记子任务。对于子任务，Rollup 字段指示子任务甘特条的信息是否会汇总到汇总任务条。对于汇总任务，Rollup 字段指示汇总任务条是否显示已汇总的条形。必须将汇总任务的 Rollup 字段设置为 Yes，子任务才能汇总到它们上。 |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | 获取或设置如果使用此保存选项对象，文档将被保存的格式。 |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate/) { get; set; } | 获取或设置渲染开始的日期。 |
| [TaskLinkDrawingCallback](../../aspose.tasks.saving/saveoptions/tasklinkdrawingcallback/) { get; set; } | 获取或设置可用于自定义任务链接渲染某些方面的回调。 |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | 获取或设置用于在甘特图和任务表图上排序任务的比较器。 |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | 获取或设置用于过滤在甘特图、任务表和任务使用图上渲染的任务的条件。 |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles/) { get; set; } | 获取或设置在项目视图渲染期间应用的文本样式列表。 |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale/) { get; set; } | 获取或设置[`Timescale`](../saveoptions/timescale/)值，该值用于控制项目保存为图形格式时时间刻度（如果存在）如何渲染。 |
| [TimescaleFitBehavior](../../aspose.tasks.saving/saveoptions/timescalefitbehavior/) { get; set; } | 获取或设置定义如何将时间刻度的右端与页面末端对齐的行为。 |
| override [UseGradientBrush](../../aspose.tasks.saving/htmlsaveoptions/usegradientbrush/) { get; set; } | 获取或设置指示在渲染项目布局时是否使用渐变画刷的值。目前在渲染为 HTML 时不支持使用渐变画刷。 |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | 获取或设置要渲染的视图列列表（[`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)）。如果未设置，则仅渲染任务 ID、任务名称、开始和结束。如果同时设置了 View 和 [`ViewSettings`](../saveoptions/viewsettings/) 属性，则 View 中的列会覆盖 ViewSettings 中的列。 |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | 获取或设置要渲染的视图（[`View`](../saveoptions/view/)）。您可以使用此选项显式指定应保存为 PDF、HTML 或图像格式的视图。如果设置了此属性，保存项目时会忽略[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/)属性。视图应来自以下其中一个屏幕（([`Screen`](../../aspose.tasks/view/screen/))）：（Gantt、TaskSheet、TaskUsage、ResourceSheet、ResourceUsage） |

## 示例

展示如何将项目保存为 HTML 格式。

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var option = new HtmlSaveOptions();
project.Save(OutDir + "SaveProjectDataAsHTML_out.html", option);

// 或

// 仅添加一页（第 2 页）
option = new HtmlSaveOptions();
option.Pages.Add(2);
project.Save(OutDir + "SaveProjectDataAsHTML2_out.html", option);
```

### 另见

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


