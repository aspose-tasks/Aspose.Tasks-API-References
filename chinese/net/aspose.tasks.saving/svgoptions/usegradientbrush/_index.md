---
title: "SvgOptions.UseGradientBrush"
second_title: "Aspose.Tasks for .NET API 参考"
description: "SvgOptions 属性。确定在渲染项目布局时是否使用渐变画刷。目前不支持在渲染为 SVG 时使用渐变画刷"
type: docs
weight: 30
url: /zh/net/aspose.tasks.saving/svgoptions/usegradientbrush/
---
## SvgOptions.UseGradientBrush property

确定在渲染项目布局时是否使用渐变画笔。目前不支持在渲染为 SVG 时使用渐变画笔。

```csharp
public override bool UseGradientBrush { get; set; }
```

## 示例

展示如何将项目保存为 SVG 文件。

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
SaveOptions options = new SvgOptions
                        {
                            // 设置文档将被保存的 <see cref=\"P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat\" />
                            PresentationFormat = PresentationFormat.GanttChart,

                            // 设置一个值，指示是否应增加行高以适应其内容
                            FitContent = true,

                            // 设置渲染的最小时间段。默认值为 <see cref=\"P:Aspose.Tasks.Saving.SaveOptions.Timescale\">Days</see>
                            Timescale = Timescale.ThirdsOfMonths,

                            // 确定在渲染项目布局时是否使用渐变画笔
                            // 目前不支持在渲染为 SVG 时使用渐变画笔。
                            // UseGradientBrush = true
                        };
project.Save(OutDir + "UseSvgOptions_out.svg", options);
```

### 另见

* class [SvgOptions](../)
* namespace [Aspose.Tasks.Saving](../../svgoptions/)
* assembly [Aspose.Tasks](../../../)


