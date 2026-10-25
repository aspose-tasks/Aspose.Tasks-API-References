---
title: "TimescaleFitBehavior"
second_title: "Aspose.Tasks for Java API Reference"
description: "시간 눈금 영역을 페이지 너비에 맞추는 동작을 나타냅니다."
type: docs
weight: 324
url: /ko/java/com.aspose.tasks/timescalefitbehavior/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class TimescaleFitBehavior extends System.Enum
```

시간 눈금 영역을 페이지 너비에 맞추는 동작을 나타냅니다.
## 필드

| 필드 | 설명 |
| --- | --- |
| [DefinedInView](#DefinedInView) | 캘린더 섹션은 렌더링된 View의 View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage 속성에 따라 렌더링됩니다. |
| [NoScaleToEndDate](#NoScaleToEndDate) | 캘린더 섹션은 페이지에 빈 공간이 있더라도 EndDate까지 정확히 렌더링됩니다. |
| [NoScaleToEndOfPage](#NoScaleToEndOfPage) | 캘린더 섹션은 마지막 페이지의 끝(오른쪽)까지 렌더링됩니다. |
| [ScaleToEndOfPage](#ScaleToEndOfPage) | 렌더링 엔진은 EndDate가 마지막 페이지의 끝(오른쪽)과 맞춰지도록 날짜를 정렬하려고 시도합니다. |
### DefinedInView {#DefinedInView}
```
public static final int DefinedInView
```


캘린더 섹션은 렌더링된 View의 View.PageInfo.PageViewSettings.FitTimescaleToEndOfPage 속성에 따라 렌더링됩니다.

### NoScaleToEndDate {#NoScaleToEndDate}
```
public static final int NoScaleToEndDate
```


캘린더 섹션은 페이지에 빈 공간이 있더라도 EndDate까지 정확히 렌더링됩니다.

### NoScaleToEndOfPage {#NoScaleToEndOfPage}
```
public static final int NoScaleToEndOfPage
```


캘린더 섹션은 마지막 페이지의 끝(오른쪽)까지 렌더링됩니다. 따라서 마지막으로 렌더링된 날짜가 EndDate를 초과할 수 있습니다.

### ScaleToEndOfPage {#ScaleToEndOfPage}
```
public static final int ScaleToEndOfPage
```


렌더링 엔진은 날짜를 정렬하려고 시도하여 EndDate가 마지막 페이지의 끝(오른쪽)과 정렬되도록 합니다. 이는 MS Project의 "Page Setup \\ View \\ Fit timescale to end of page" 옵션이 활성화된 것과 같습니다.

