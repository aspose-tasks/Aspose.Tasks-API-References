---
title: PdfSaveOptions
second_title: Aspose.Tasks for .NET API 参考
description: 允许在将项目页面呈现为 PDF 时指定其他选项
type: docs
weight: 1850
url: /zh/net/aspose.tasks.saving/pdfsaveoptions/
---
## PdfSaveOptions class

允许在将项目页面呈现为 PDF 时指定其他选项。

```csharp
public class PdfSaveOptions : SaveOptions
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions)() | 初始化[`PdfSaveOptions`](../pdfsaveoptions)可用于将文档保存在[`PDF格式`](../savefileformat)格式。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles) { get; set; } | 获取或设置实例的列表[`BarStyle`](../../aspose.tasks.visualization/barstyle)出现在项目视图中的类。 |
| [Compliance](../../aspose.tasks.saving/pdfsaveoptions/compliance) { get; set; } | 获取或设置生成的 PDF 文档所需的合规级别。 默认为Pdf15. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize) { get; set; } | 获取或设置以磅为单位的自定义页面大小（1 磅 = 1/72 英寸）。 |
| [DefaultFontName](../../aspose.tasks.saving/pdfsaveoptions/defaultfontname) { get; set; } | 获取或设置渲染的默认字体。 |
| [DigitalSignatureDetails](../../aspose.tasks.saving/pdfsaveoptions/digitalsignaturedetails) { get; set; } | 获取或设置数字签名详细信息。如果未设置，则不会执行签名。 |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime) { get; set; } | 获取或设置一个值，指示是否应绘制非工作时间（默认值为 TRUE）。 |
| [EncryptionDetails](../../aspose.tasks.saving/pdfsaveoptions/encryptiondetails) { get; set; } | 获取或设置加密细节。如果未设置，则不会执行加密。 |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate) { get; set; } | 获取或设置完成渲染的日期。 |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent) { get; set; } | 获取或设置一个值，该值指示是否应增加行高以适应其内容。 |
| [FontResolveCallback](../../aspose.tasks.saving/pdfsaveoptions/fontresolvecallback) { get; set; } | 获取或设置可用于自定义已解析字体的回调。 |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines) { get; set; } | 获取或设置列表[`Gridline`](../../aspose.tasks.visualization/gridline)出现在项目视图中。 |
| [LegendOnEachPage](../../aspose.tasks.saving/saveoptions/legendoneachpage) { get; set; } | 获取或设置一个值，该值指示是否应在每页上显示图例（默认值为 TRUE）。 |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks) { get; set; } | 获取或设置一个值，该值指示关键任务是否应以红色显示（默认值为 FALSE）。 |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor) { get; set; } | 获取或设置非工作时间颜色。 |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount) { get; } | 获取或设置项目的页数。 |
| [Pages](../../aspose.tasks.saving/pdfsaveoptions/pages) { get; set; } | 获取或设置将项目布局保存到单独文件时要保存的页码列表。 如果此列表为空，则将保存所有页面。 |
| [PageSavingCallback](../../aspose.tasks.saving/pdfsaveoptions/pagesavingcallback) { get; set; } | 获取或设置用户定义的回调，用于获取每个渲染页面的输出流。 适用于[`SaveToSeparateFiles`](./savetoseparatefiles)使用选项。 |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize) { get; set; } | 获取或设置要渲染的页面大小（默认值为PageSize.A4）。 |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat) { get; set; } | 获取或设置[`PresentationFormat`](../saveoptions/presentationformat)文档将保存在其中。 |
| [ReduceFooterGap](../../aspose.tasks.saving/pdfsaveoptions/reducefootergap) { get; set; } | 获取或设置一个值，该值指示是否必须缩小最后一个任务和页脚之间的间隙。 |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage) { get; set; } | 获取或设置一个值，该值指示项目是否应呈现为单个页面 当项目以图形格式保存时。 页面大小将更改，以便呈现的项目可以放在一页上。 |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars) { get; set; } | 获取或设置一个值，该值指示是否应标记摘要任务栏上的子任务。 对于子任务，Rollup 字段指示是否将子任务甘特条上的信息汇总到摘要任务栏。 对于摘要任务，Rollup字段指示摘要任务栏是否显示汇总栏。 您必须将摘要任务的汇总字段设置为是，以便任何子任务汇总到它们。 |
| [SaveFormat](../../aspose.tasks.saving/saveoptions/saveformat) { get; } | 获取或设置在使用此保存选项对象时保存文档的格式。 |
| [SaveToSeparateFiles](../../aspose.tasks.saving/pdfsaveoptions/savetoseparatefiles) { get; set; } | 获取或设置一个值，该值指示是否将项目页面保存到单独的文件中。 |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate) { get; set; } | 获取或设置开始渲染的日期。 |
| [TasksComparer](../../aspose.tasks.saving/saveoptions/taskscomparer) { get; set; } | 获取或设置比较器以对甘特图和任务表上的任务进行排序。 |
| [TasksFilter](../../aspose.tasks.saving/saveoptions/tasksfilter) { get; set; } | 获取或设置用于过滤在甘特图、任务表和任务使用图表上呈现的任务的条件。 |
| [TextCompression](../../aspose.tasks.saving/pdfsaveoptions/textcompression) { get; set; } | 获取或设置用于除图像之外的所有内容流的压缩类型。 默认为Flate. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles) { get; set; } | 获取或设置实例的列表[`TextStyle`](../../aspose.tasks.visualization/textstyle)出现在项目视图中的类。 |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale) { get; set; } | 获取或设置[`Timescale`](../saveoptions/timescale)用于控制将项目保存为图形格式时如何呈现时间刻度（如果存在）的值。 |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush) { get; set; } | 获取或设置一个值，该值指示渲染甘特图时是否应使用渐变画笔。 |
| [UseProjectDefaultFont](../../aspose.tasks.saving/pdfsaveoptions/useprojectdefaultfont) { get; set; } | 获取或设置一个值，该值指示是否必须使用默认字体进行渲染。 |
| [View](../../aspose.tasks.saving/saveoptions/view) { get; set; } | 获取或设置要渲染的视图列列表 ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn) ). 如果未设置，则仅呈现任务 ID、任务名称、开始和完成。 如果查看和[`ViewSettings`](../saveoptions/viewsettings)属性已设置，View 中的列会覆盖 ViewSettings. 中的列 |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings) { get; set; } | 获取或设置视图 ([`View`](../saveoptions/view)） 渲染。您可以使用此选项明确指定应将哪个视图保存为 PDF、HTML 或图像格式。 如果设置了此属性，[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat)保存项目时忽略属性。 视图应来自以下屏幕之一（（[`Screen`](../../aspose.tasks/view/screen) )): (甘特图、TaskSheet、TaskUsage、ResourceSheet、ResourceUsage) |

### 也可以看看

* class [SaveOptions](../saveoptions)
* 命名空间 [Aspose.Tasks.Saving](../../aspose.tasks.saving)
* 部件 [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
