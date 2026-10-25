---
title: "UsageView"
second_title: "Aspose.Tasks for Java API Reference"
description: "프로젝트에서 사용 보기를 나타냅니다."
type: docs
weight: 331
url: /ko/java/com.aspose.tasks/usageview/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.View](../../com.aspose.tasks/view)

**All Implemented Interfaces:**
com.aspose.tasks.ITimescaledView
```
public abstract class UsageView extends View implements ITimescaledView
```

프로젝트에서 사용 보기를 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getAlignDetailsData()](#getAlignDetailsData--) | 세부 데이터 정렬을 가져옵니다. |
| [getBottomTimescaleTier()](#getBottomTimescaleTier--) | 뷰의 하단 타임스케일 계층 설정을 가져옵니다. |
| [getDisplayDetailsHeaderColumn()](#getDisplayDetailsHeaderColumn--) | 뷰에 세부 헤더 열을 표시할지 여부를 나타내는 값을 가져옵니다. |
| [getDisplayShortDetailHeaderNames()](#getDisplayShortDetailHeaderNames--) | 짧은 세부 헤더 이름을 표시할지 여부를 나타내는 값을 가져옵니다. |
| [getMiddleTimescaleTier()](#getMiddleTimescaleTier--) | 뷰의 중간 타임스케일 계층 설정을 가져옵니다. |
| [getRepeatDetailsHeaderOnAllRows()](#getRepeatDetailsHeaderOnAllRows--) | 모든 할당 행에 세부 헤더를 반복할지 여부를 나타내는 값을 가져옵니다. |
| [getTimescaleSizePercentage()](#getTimescaleSizePercentage--) | \{@inheritDoc\} |
| [getTopTimescaleTier()](#getTopTimescaleTier--) | 뷰의 상단 타임스케일 계층 설정을 가져옵니다. |
| [setAlignDetailsData(int value)](#setAlignDetailsData-int-) | 세부 데이터 정렬을 설정합니다. |
| [setBottomTimescaleTier(TimescaleTier value)](#setBottomTimescaleTier-com.aspose.tasks.TimescaleTier-) | 뷰의 하단 타임스케일 계층 설정을 설정합니다. |
| [setDisplayDetailsHeaderColumn(boolean value)](#setDisplayDetailsHeaderColumn-boolean-) | 뷰에 세부 헤더 열을 표시할지 여부를 나타내는 값을 설정합니다. |
| [setDisplayShortDetailHeaderNames(boolean value)](#setDisplayShortDetailHeaderNames-boolean-) | 짧은 세부 헤더 이름을 표시할지 여부를 나타내는 값을 설정합니다. |
| [setMiddleTimescaleTier(TimescaleTier value)](#setMiddleTimescaleTier-com.aspose.tasks.TimescaleTier-) | 보기의 중간 타임스케일 계층 설정을 지정합니다. |
| [setRepeatDetailsHeaderOnAllRows(boolean value)](#setRepeatDetailsHeaderOnAllRows-boolean-) | 모든 할당 행에 상세 헤더를 반복할지 여부를 나타내는 값을 설정합니다. |
| [setTimescaleSizePercentage(int value)](#setTimescaleSizePercentage-int-) | \{@inheritDoc\} |
| [setTopTimescaleTier(TimescaleTier value)](#setTopTimescaleTier-com.aspose.tasks.TimescaleTier-) | 보기의 상단 타임스케일 계층 설정을 지정합니다. |
### getAlignDetailsData() {#getAlignDetailsData--}
```
public final int getAlignDetailsData()
```


세부 데이터 정렬을 가져옵니다.

**Returns:**
int - 상세 데이터 정렬.
### getBottomTimescaleTier() {#getBottomTimescaleTier--}
```
public final TimescaleTier getBottomTimescaleTier()
```


보기의 하단 타임스케일 계층 설정을 가져옵니다. [TimescaleTier](../../com.aspose.tasks/timescaletier)

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's bottom timescale tier.
### getDisplayDetailsHeaderColumn() {#getDisplayDetailsHeaderColumn--}
```
public final boolean getDisplayDetailsHeaderColumn()
```


뷰에 세부 헤더 열을 표시할지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 보기에서 상세 헤더 열을 표시할지 여부를 나타내는 값.
### getDisplayShortDetailHeaderNames() {#getDisplayShortDetailHeaderNames--}
```
public final boolean getDisplayShortDetailHeaderNames()
```


짧은 세부 헤더 이름을 표시할지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 짧은 상세 헤더 이름을 표시할지 여부를 나타내는 값.
### getMiddleTimescaleTier() {#getMiddleTimescaleTier--}
```
public final TimescaleTier getMiddleTimescaleTier()
```


보기의 중간 타임스케일 계층 설정을 가져옵니다. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's middle timescale tier.
### getRepeatDetailsHeaderOnAllRows() {#getRepeatDetailsHeaderOnAllRows--}
```
public final boolean getRepeatDetailsHeaderOnAllRows()
```


모든 할당 행에 세부 헤더를 반복할지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 모든 할당 행에 상세 헤더를 반복할지 여부를 나타내는 값.
### getTimescaleSizePercentage() {#getTimescaleSizePercentage--}
```
public final int getTimescaleSizePercentage()
```


타임스케일 계층에서 단위 간 간격을 줄이거나 늘릴 비율을 가져옵니다.

**Returns:**
int - \{@inheritDoc\}
### getTopTimescaleTier() {#getTopTimescaleTier--}
```
public final TimescaleTier getTopTimescaleTier()
```


보기의 상단 타임스케일 계층 설정을 가져옵니다. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's top timescale tier.
### setAlignDetailsData(int value) {#setAlignDetailsData-int-}
```
public final void setAlignDetailsData(int value)
```


세부 데이터 정렬을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 상세 데이터 정렬. |

### setBottomTimescaleTier(TimescaleTier value) {#setBottomTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setBottomTimescaleTier(TimescaleTier value)
```


보기의 하단 타임스케일 계층 설정을 지정합니다. [TimescaleTier](../../com.aspose.tasks/timescaletier)

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | 보기의 하단 타임스케일 계층 설정. |

### setDisplayDetailsHeaderColumn(boolean value) {#setDisplayDetailsHeaderColumn-boolean-}
```
public final void setDisplayDetailsHeaderColumn(boolean value)
```


뷰에 세부 헤더 열을 표시할지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 보기에서 상세 헤더 열을 표시할지 여부를 나타내는 값. |

### setDisplayShortDetailHeaderNames(boolean value) {#setDisplayShortDetailHeaderNames-boolean-}
```
public final void setDisplayShortDetailHeaderNames(boolean value)
```


짧은 세부 헤더 이름을 표시할지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 짧은 상세 헤더 이름을 표시할지 여부를 나타내는 값. |

### setMiddleTimescaleTier(TimescaleTier value) {#setMiddleTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setMiddleTimescaleTier(TimescaleTier value)
```


보기의 중간 타임스케일 계층 설정을 지정합니다. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | 보기의 중간 타임스케일 계층 설정. |

### setRepeatDetailsHeaderOnAllRows(boolean value) {#setRepeatDetailsHeaderOnAllRows-boolean-}
```
public final void setRepeatDetailsHeaderOnAllRows(boolean value)
```


모든 할당 행에 상세 헤더를 반복할지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 모든 할당 행에 상세 헤더를 반복할지 여부를 나타내는 값. |

### setTimescaleSizePercentage(int value) {#setTimescaleSizePercentage-int-}
```
public final void setTimescaleSizePercentage(int value)
```


타임스케일 계층에서 단위 간 간격을 줄이거나 늘릴 비율을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | \{@inheritDoc\} |

### setTopTimescaleTier(TimescaleTier value) {#setTopTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setTopTimescaleTier(TimescaleTier value)
```


보기의 상단 타임스케일 계층 설정을 지정합니다. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | 보기의 상단 타임스케일 계층 설정. |

