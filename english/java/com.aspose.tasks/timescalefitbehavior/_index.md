---
title: TimescaleFitBehavior
second_title: Aspose.Tasks for Java API Reference
description: Represents a behavior used to align timescale area with page width.
type: docs
weight: 323
url: /java/com.aspose.tasks/timescalefitbehavior/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class TimescaleFitBehavior extends System.Enum
```

Represents a behavior used to align timescale area with page width.
## Fields

| Field | Description |
| --- | --- |
| [DefinedInView](#DefinedInView) | Calendar section is rendered according to View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage property of the rendered View. |
| [NoScaleToEndDate](#NoScaleToEndDate) | Calendar section is rendered exactly to EndDate, even there is an empty space on a page. |
| [NoScaleToEndOfPage](#NoScaleToEndOfPage) | Calendar section is rendered to the end (right side) of the last page. |
| [ScaleToEndOfPage](#ScaleToEndOfPage) | Rendering engine will try to align dates so that EndDate is aligned with the end (right side) of the last page. |
### DefinedInView {#DefinedInView}
```
public static final int DefinedInView
```


Calendar section is rendered according to View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage property of the rendered View.

### NoScaleToEndDate {#NoScaleToEndDate}
```
public static final int NoScaleToEndDate
```


Calendar section is rendered exactly to EndDate, even there is an empty space on a page.

### NoScaleToEndOfPage {#NoScaleToEndOfPage}
```
public static final int NoScaleToEndOfPage
```


Calendar section is rendered to the end (right side) of the last page. Thus last rendered date may exceed EndDate.

### ScaleToEndOfPage {#ScaleToEndOfPage}
```
public static final int ScaleToEndOfPage
```


Rendering engine will try to align dates so that EndDate is aligned with the end (right side) of the last page. Corresponds to MS Project's "Page Setup \\ View \\ Fit timescale to end of page" option enabled.

