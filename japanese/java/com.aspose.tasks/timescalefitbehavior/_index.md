---
title: "TimescaleFitBehavior"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "ページ幅に合わせてタイムスケール領域を揃えるために使用される動作を表します。"
type: docs
weight: 324
url: /ja/java/com.aspose.tasks/timescalefitbehavior/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class TimescaleFitBehavior extends System.Enum
```

ページ幅に合わせてタイムスケール領域を揃えるために使用される動作を表します。
## フィールド

| フィールド | 説明 |
| --- | --- |
| [DefinedInView](#DefinedInView) | カレンダー セクションは、レンダリングされたビューの View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage プロパティに従って描画されます。 |
| [NoScaleToEndDate](#NoScaleToEndDate) | カレンダー セクションは、ページに空白があっても EndDate まで正確に描画されます。 |
| [NoScaleToEndOfPage](#NoScaleToEndOfPage) | カレンダー セクションは最終ページの末端（右側）まで描画されます。 |
| [ScaleToEndOfPage](#ScaleToEndOfPage) | レンダリング エンジンは、EndDate が最終ページの末端（右側）に合わせられるように日付を調整しようとします。 |
### DefinedInView {#DefinedInView}
```
public static final int DefinedInView
```


カレンダー セクションは、レンダリングされたビューの View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage プロパティに従って描画されます。

### NoScaleToEndDate {#NoScaleToEndDate}
```
public static final int NoScaleToEndDate
```


カレンダー セクションは、ページに空白があっても EndDate まで正確に描画されます。

### NoScaleToEndOfPage {#NoScaleToEndOfPage}
```
public static final int NoScaleToEndOfPage
```


カレンダー セクションは最終ページの末端（右側）まで描画されます。そのため、最後に描画された日付が EndDate を超える可能性があります。

### ScaleToEndOfPage {#ScaleToEndOfPage}
```
public static final int ScaleToEndOfPage
```


レンダリングエンジンは、日付を最後のページの末尾（右側）に合わせるように EndDate を揃えようとします。MS Project の「Page Setup \\ View \\ Fit timescale to end of page」オプションが有効になっていることに対応します。

