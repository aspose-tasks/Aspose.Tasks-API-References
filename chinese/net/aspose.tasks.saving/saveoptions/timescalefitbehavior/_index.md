---
title: "SaveOptions.TimescaleFitBehavior"
second_title: "Aspose.Tasks for .NET API 参考"
description: "SaveOptions 属性。获取或设置一种行为，定义如何将时间轴的右端与页面末端对齐"
type: docs
weight: 210
url: /zh/net/aspose.tasks.saving/saveoptions/timescalefitbehavior/
---
## SaveOptions.TimescaleFitBehavior property

获取或设置定义如何将时间刻度的右端与页面末端对齐的行为。

```csharp
public TimescaleFitBehavior TimescaleFitBehavior { get; set; }
```

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

* enum [TimescaleFitBehavior](../../../aspose.tasks.visualization/timescalefitbehavior/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


