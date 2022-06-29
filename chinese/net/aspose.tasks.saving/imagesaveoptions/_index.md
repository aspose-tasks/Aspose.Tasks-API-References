---
title: ImageSaveOptions
second_title: Aspose.Tasks for .NET API 参考
description: 允许在将项目页面渲染为图像时指定其他选项
type: docs
weight: 1760
url: /zh/net/aspose.tasks.saving/imagesaveoptions/
---
## ImageSaveOptions class

允许在将项目页面渲染为图像时指定其他选项。

```csharp
public class ImageSaveOptions : SaveOptions
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [ImageSaveOptions](imagesaveoptions)(SaveFileFormat) | 初始化[`ImageSaveOptions`](../imagesaveoptions)类的新实例，该类可用于在 TIFF 中保存渲染图像， PNG、BMP 或 JPEG 格式。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles) { get; set; } | 获取或设置项目视图中出现的[`BarStyle`](../../aspose.tasks.visualization/barstyle)类的实例列表。 |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize) { get; set; } | 获取或设置以磅为单位的自定义页面大小（1 磅 = 1/72 英寸）。 |
| [DefaultFontName](../../aspose.tasks.saving/imagesaveoptions/defaultfontname) { get; set; } | 获取或设置渲染的默认字体。 |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime) { get; set; } | 获取或设置一个指示是否应绘制非工作时间的值（默认值为 TRUE）。 |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate) { get; set; } | 获取或设置完成渲染的日期。 |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent) { get; set; } | 获取或设置一个值，该值指示是否应增加行高以适合其内容。 |
| [FontResolveCallback](../../aspose.tasks.saving/imagesaveoptions/fontresolvecallback) { get; set; } | 获取或设置可用于自定义已解析字体的回调。 |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines) { get; set; } | 获取或设置项目视图中出现的[`Gridline`](../../aspose.tasks.visualization/gridline)列表。 |
| [HorizontalResolution](../../aspose.tasks.saving/imagesaveoptions/horizontalresolution) { get; set; } | 获取或设置水平分辨率，以 dpi 为单位。 |
| [JpegQuality](../../aspose.tasks.saving/imagesaveoptions/jpegquality) { get; set; } | 获取或设置 JPEG 质量。允许的值范围是 0..100。 |
| [LegendOnEachPage](../../aspose.tasks.saving/saveoptions/legendoneachpage) { get; set; } | 获取或设置一个值，该值指示是否应在每个页面上显示图例（默认值为 TRUE）。 |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks) { get; set; } | 获取或设置一个值，该值指示关键任务是否应以红色显示（默认值为 FALSE）。 |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor) { get; set; } | 获取或设置非工作时间颜色。 |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount) { get; } | 获取或设置项目页数。 |
| [Pages](../../aspose.tasks.saving/imagesaveoptions/pages) { get; set; } | 获取或设置将项目布局保存到单独文件时要保存的页码列表。  如果此列表为空，则将保存所有页面。 |
| [PageSavingCallback](../../aspose.tasks.saving/imagesaveoptions/pagesavingcallback) { get; set; } | 获取或设置用户定义的回调，用于获取每个渲染页面的输出流。 |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize) { get; set; } | 获取或设置要呈现的页面大小（默认值为 PageSize.A4）。 |
| [PixelFormat](../../aspose.tasks.saving/imagesaveoptions/pixelformat) { get; set; } | 获取或设置图像中每个像素的颜色数据格式。 |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat) { get; set; } | 获取或设置保存文档的[`PresentationFormat`](../saveoptions/presentationformat)。 |
| [ReduceFooterGap](../../aspose.tasks.saving/imagesaveoptions/reducefootergap) { get; set; } | 获取或设置一个值，该值指示是否必须缩小最后一个任务和页脚之间的间隙。 |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage) { get; set; } | 获取或设置一个值，该值指示在以图形格式保存项目时是否应将项目呈现到单个页面 。 页面大小将被更改，因此渲染的项目可以放在一页上。 |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars) { get; set; } | 获取或设置一个值，该值指示是否应标记摘要任务栏上的子任务。 对于子任务，Rollup 字段指示是否将子任务甘特条上的信息汇总到摘要任务栏。 对于汇总任务，汇总字段指示汇总任务栏是否显示汇总条。 您必须将汇总任务的汇总字段设置为是，以便任何子任务汇总到它们。 |
| [SaveFormat](../../aspose.tasks.saving/saveoptions/saveformat) { get; } | 获取或设置在使用此保存选项对象时保存文档的格式。 |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate) { get; set; } | 获取或设置开始渲染的日期。 |
| [TasksComparer](../../aspose.tasks.saving/saveoptions/taskscomparer) { get; set; } | 获取或设置比较器以对甘特图和任务表上的任务进行排序。 |
| [TasksFilter](../../aspose.tasks.saving/saveoptions/tasksfilter) { get; set; } | 获取或设置用于过滤在甘特图、任务表和任务使用图表上呈现的任务的条件。 |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles) { get; set; } | 获取或设置项目视图中出现的[`TextStyle`](../../aspose.tasks.visualization/textstyle)类的实例列表。 |
| [TiffCompression](../../aspose.tasks.saving/imagesaveoptions/tiffcompression) { get; set; } | 获取或设置将生成的图像保存为 TIFF 格式时应用的压缩类型。 |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale) { get; set; } | 获取或设置[`Timescale`](../saveoptions/timescale)值，用于控制时间刻度（如果存在）在项目保存为图形格式时呈现。 |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush) { get; set; } | 获取或设置一个值，该值指示在渲染甘特图时是否应使用渐变画笔。 |
| [UseProjectDefaultFont](../../aspose.tasks.saving/imagesaveoptions/useprojectdefaultfont) { get; set; } | 获取或设置一个值，该值指示是否必须使用默认字体进行渲染。 |
| [VerticalResolution](../../aspose.tasks.saving/imagesaveoptions/verticalresolution) { get; set; } | 获取或设置 dpi 的垂直分辨率。 |
| [View](../../aspose.tasks.saving/saveoptions/view) { get; set; } | 获取或设置要呈现的视图列的列表（[`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn)）。 如果未设置，则仅呈现任务 ID、任务名称、开始和完成。 如果同时设置了 View 和[`ViewSettings`](../saveoptions/viewsettings)属性，则 View 中的列将覆盖 ViewSettings 中的列。 |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings) { get; set; } | 获取或设置要渲染的视图（[`View`](../saveoptions/view)）。您可以使用此选项明确指定应将哪个视图保存为 PDF、HTML 或图像格式。 如果设置了此属性，则保存项目时将忽略[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat)属性。 视图应来自以下屏幕之一（（[`Screen`](../../aspose.tasks/view/screen)））:（甘特图，TaskSheet，TaskUsage，ResourceSheet，ResourceUsage） |

### 也可以看看

* class [SaveOptions](../saveoptions)
* 命名空间 [Aspose.Tasks.Saving](../../aspose.tasks.saving)
* 部件 [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
