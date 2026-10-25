---
title: "SaveOptions.TimescaleFitBehavior"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "SaveOptions プロパティ。タイムスケールの右端をページの末端に合わせる方法を定義する動作を取得または設定します"
type: docs
weight: 210
url: /ja/net/aspose.tasks.saving/saveoptions/timescalefitbehavior/
---
## SaveOptions.TimescaleFitBehavior property

タイムスケールの右端をページの末端に合わせる方法を定義する動作を取得または設定します。

```csharp
public TimescaleFitBehavior TimescaleFitBehavior { get; set; }
```

## 例

TimescaleFitBehavior を使用してガントチャートのタイムスケールを最終ページの末端に合わせる方法を示します。

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

### 関連項目

* enum [TimescaleFitBehavior](../../../aspose.tasks.visualization/timescalefitbehavior/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


