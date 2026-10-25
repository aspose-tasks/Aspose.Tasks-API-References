---
title: "Enum TimescaleFitBehavior"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "Aspose.Tasks.Visualization.TimescaleFitBehavior enum. タイムスケール領域をページ幅に合わせて配置する動作を表します"
type: docs
weight: 3440
url: /ja/net/aspose.tasks.visualization/timescalefitbehavior/
---
## TimescaleFitBehavior enumeration

タイムスケール領域をページ幅に合わせて配置する動作を表します。

```csharp
public enum TimescaleFitBehavior
```

### 値

| 名前 | 値 | 説明 |
| --- | --- | --- |
| DefinedInView | `0` | カレンダー セクションは、レンダリングされたビューの View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage プロパティに従って描画されます。 |
| NoScaleToEndDate | `1` | カレンダー セクションはページに空白があっても、EndDate まで正確に描画されます。 |
| NoScaleToEndOfPage | `2` | カレンダー セクションは最終ページの末端（右側）まで描画されます。そのため、最後に描画された日付が EndDate を超えることがあります。 |
| ScaleToEndOfPage | `3` | レンダリング エンジンは、EndDate が最終ページの末端（右側）に揃うように日付を調整しようとします。これは、MS Project の「ページ設定 \ ビュー \ タイムスケールをページの末端に合わせる」オプションが有効になっている状態に相当します。 |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


