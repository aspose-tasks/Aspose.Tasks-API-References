---
title: "SvgOptions.SvgOptions"
second_title: "Aspose.Tasks for .NET API 参考"
description: "SvgOptions 构造函数。初始化 SvgOptions 类的新实例，可用于以 SVG 格式保存项目"
type: docs
weight: 10
url: /zh/net/aspose.tasks.saving/svgoptions/svgoptions/
---
## SvgOptions constructor

初始化 [`SvgOptions`](../) 类的新实例，可用于以 SVG 格式保存项目。

```csharp
public SvgOptions()
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


