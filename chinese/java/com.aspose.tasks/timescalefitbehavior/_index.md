---
title: "TimescaleFitBehavior"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示用于将时间尺度区域与页面宽度对齐的行为。"
type: docs
weight: 324
url: /zh/java/com.aspose.tasks/timescalefitbehavior/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class TimescaleFitBehavior extends System.Enum
```

表示用于将时间尺度区域与页面宽度对齐的行为。
## 字段

| 字段 | 描述 |
| --- | --- |
| [DefinedInView](#DefinedInView) | 日历部分根据渲染视图的 View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage 属性进行渲染。 |
| [NoScaleToEndDate](#NoScaleToEndDate) | 日历部分精确渲染至 EndDate，即使页面上有空白空间。 |
| [NoScaleToEndOfPage](#NoScaleToEndOfPage) | 日历部分渲染至最后一页的末端（右侧）。 |
| [ScaleToEndOfPage](#ScaleToEndOfPage) | 渲染引擎将尝试对齐日期，使 EndDate 与最后一页的末端（右侧）对齐。 |
### DefinedInView {#DefinedInView}
```
public static final int DefinedInView
```


日历部分根据渲染视图的 View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage 属性进行渲染。

### NoScaleToEndDate {#NoScaleToEndDate}
```
public static final int NoScaleToEndDate
```


日历部分精确渲染至 EndDate，即使页面上有空白空间。

### NoScaleToEndOfPage {#NoScaleToEndOfPage}
```
public static final int NoScaleToEndOfPage
```


日历部分渲染至最后一页的末端（右侧）。因此，最后渲染的日期可能会超过 EndDate。

### ScaleToEndOfPage {#ScaleToEndOfPage}
```
public static final int ScaleToEndOfPage
```


渲染引擎将尝试对齐日期，使 EndDate 与最后一页的末端（右侧）对齐。对应于已启用 MS Project 的 "Page Setup \\ View \\ Fit timescale to end of page" 选项。

