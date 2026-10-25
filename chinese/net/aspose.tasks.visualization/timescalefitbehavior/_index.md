---
title: "枚举 TimescaleFitBehavior"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Visualization.TimescaleFitBehavior 枚举。表示用于将时间尺度区域与页面宽度对齐的行为"
type: docs
weight: 3440
url: /zh/net/aspose.tasks.visualization/timescalefitbehavior/
---
## TimescaleFitBehavior enumeration

表示用于将时间尺度区域与页面宽度对齐的行为。

```csharp
public enum TimescaleFitBehavior
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| DefinedInView | `0` | 日历部分根据渲染视图的 View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage 属性进行渲染。 |
| NoScaleToEndDate | `1` | 日历部分精确渲染到 EndDate，即使页面上有空白空间。 |
| NoScaleToEndOfPage | `2` | 日历部分渲染到最后一页的末端（右侧）。因此最后渲染的日期可能超过 EndDate。 |
| ScaleToEndOfPage | `3` | 渲染引擎将尝试对齐日期，使 EndDate 与最后一页的末端（右侧）对齐。对应于启用的 MS Project “页面设置 \ 视图 \ 将时间尺度适配到页面末端” 选项。 |

## 示例

展示如何使用 TimescaleFitBehavior 使甘特图的时间尺度适配到最后一页的末端。

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

var view = project.DefaultView as GanttChartView;

PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.PageSize = PageSize.A4;
saveOptions.StartDate = project.StartDate;
saveOptions.EndDate = project.FinishDate;
saveOptions.ViewSettings = view;
saveOptions.TimescaleFitBehavior = TimescaleFitBehavior.ScaleToEndOfPage;

project.Save(OutDir + "WorkWithPageSizeDefinedInView_out.pdf", saveOptions);
```

### 另见

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


