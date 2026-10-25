---
title: "枚举 Timescale"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Visualization.Timescale 枚举。定义选项，指定在项目导出为图形格式时，如何在甘特图任务使用或资源使用视图中呈现时间刻度。"
type: docs
weight: 3430
url: /zh/net/aspose.tasks.visualization/timescale/
---
## Timescale enumeration

定义选项，以指定在项目导出为图形格式时，如何在甘特图、任务使用或资源使用视图中呈现时间尺度。

```csharp
public enum Timescale
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| DefinedInView | `0` | 使用在项目视图属性中定义的时间刻度设置：[`BottomTimescaleTier`](../../aspose.tasks/ganttchartview/bottomtimescaletier/)、[`MiddleTimescaleTier`](../../aspose.tasks/ganttchartview/middletimescaletier/)、[`TopTimescaleTier`](../../aspose.tasks/ganttchartview/toptimescaletier/)。适用于包含视图数据的格式。例如，从 MPP 格式读取的项目。 |
| Days | `1` | 预定义的两层时间刻度，最小细节级别为一天。 |
| ThirdsOfMonths | `10` | 预定义的两层时间刻度，细节级别为一个月的三分之一。 |
| Months | `30` | 预定义的两层时间刻度，最小细节级别为一个月。 |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


