---
title: "TimescaleTier"
second_title: "Aspose.Tasks for Java API Reference"
description: "Gantt 차트의 시간 눈금 단일 계층을 나타냅니다."
type: docs
weight: 325
url: /ko/java/com.aspose.tasks/timescaletier/
---

**Inheritance:**
java.lang.Object
```
public final class TimescaleTier
```

Gantt 차트의 시간 눈금 단일 계층을 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [TimescaleTier()](#TimescaleTier--) | [TimescaleTier](../../com.aspose.tasks/timescaletier) 클래스의 새 인스턴스를 초기화합니다. |
| [TimescaleTier(int unit, int count)](#TimescaleTier-int-int-) | [TimescaleTier](../../com.aspose.tasks/timescaletier) 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getAlignment()](#getAlignment--) | 계층의 각 시간 기간 내에서 레이블을 정렬하는 방법을 가져옵니다 ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)). |
| [getCount()](#getCount--) | 계층에 레이블을 표시할 시간 단위 간격을 가져옵니다. |
| [getDateTimeConverter()](#getDateTimeConverter--) | 이 계층에서 날짜 틱 렌더링을 처리하기 위한 콜백 함수를 가져옵니다. |
| [getLabel()](#getLabel--) | 시간 눈금 계층에 대한 날짜 레이블 [DateLabel](../../com.aspose.tasks/datelabel)을 가져옵니다. |
| [getRenderLabelOnEachPage()](#getRenderLabelOnEachPage--) | 시간 기간이 여러 페이지에 걸칠 때 각 페이지에 날짜 레이블을 렌더링할지 여부를 정의하는 플래그를 가져옵니다. |
| [getShowTicks()](#getShowTicks--) | 계층에서 시간 기간을 구분하는 눈금 표시를 표시할지 여부를 나타내는 값을 가져옵니다. |
| [getUnit()](#getUnit--) | 시간 눈금 계층에 대한 시간 눈금 단위 [TimescaleUnit](../../com.aspose.tasks/timescaleunit)를 가져옵니다. |
| [getUsesFiscalYear()](#getUsesFiscalYear--) | 계층 레이블을 회계 연도 기준으로 할지 여부를 나타내는 값을 가져옵니다. |
| [setAlignment(int value)](#setAlignment-int-) | 계층의 각 시간 기간 내에서 레이블을 정렬하는 방법을 설정합니다 ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)). |
| [setCount(int value)](#setCount-int-) | 계층에 레이블을 표시할 시간 단위 간격을 설정합니다. |
| [setDateTimeConverter(DateTimeConverter value)](#setDateTimeConverter-com.aspose.tasks.DateTimeConverter-) | 이 계층에서 날짜 틱 렌더링을 처리하기 위한 콜백 함수를 설정합니다. |
| [setLabel(int value)](#setLabel-int-) | 시간 눈금 계층에 대한 날짜 레이블 [DateLabel](../../com.aspose.tasks/datelabel)를 설정합니다. |
| [setRenderLabelOnEachPage(boolean value)](#setRenderLabelOnEachPage-boolean-) | 시간 기간이 여러 페이지에 걸칠 때 각 페이지에 날짜 레이블을 렌더링할지 여부를 정의하는 플래그를 설정합니다. |
| [setShowTicks(boolean value)](#setShowTicks-boolean-) | 계층에서 시간 기간을 구분하는 눈금 표시를 표시할지 여부를 나타내는 값을 설정합니다. |
| [setUnit(int value)](#setUnit-int-) | 시간 눈금 계층에 대한 시간 눈금 단위 [TimescaleUnit](../../com.aspose.tasks/timescaleunit)를 설정합니다. |
| [setUsesFiscalYear(boolean value)](#setUsesFiscalYear-boolean-) | 계층 레이블을 회계 연도 기준으로 할지 여부를 나타내는 값을 설정합니다. |
### TimescaleTier() {#TimescaleTier--}
```
public TimescaleTier()
```


[TimescaleTier](../../com.aspose.tasks/timescaletier) 클래스의 새 인스턴스를 초기화합니다.

### TimescaleTier(int unit, int count) {#TimescaleTier-int-int-}
```
public TimescaleTier(int unit, int count)
```


[TimescaleTier](../../com.aspose.tasks/timescaletier) 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| unit | int | 시간 눈금 단위 [TimescaleUnit](../../com.aspose.tasks/timescaleunit)입니다. |
| count | int | [TimescaleUnit](../../com.aspose.tasks/timescaleunit) 단위의 개수입니다. |

### getAlignment() {#getAlignment--}
```
public final int getAlignment()
```


계층의 각 시간 기간 내에서 레이블을 정렬하는 방법을 가져옵니다 ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).

**Returns:**
int - 계층의 각 시간 기간 내에서 레이블을 정렬하는 방법 ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).
### getCount() {#getCount--}
```
public final int getCount()
```


계층에 레이블을 표시할 시간 단위 간격을 가져옵니다. 기본값은 1입니다.

**Returns:**
int - 계층에 레이블을 표시할 시간 단위 간격.
### getDateTimeConverter() {#getDateTimeConverter--}
```
public final DateTimeConverter getDateTimeConverter()
```


이 계층에서 날짜 틱 렌더링을 처리하기 위한 콜백 함수를 가져옵니다.

**Returns:**
[DateTimeConverter](../../com.aspose.tasks/datetimeconverter) - a callback function for handling rendering date tick in this tier.
### getLabel() {#getLabel--}
```
public final int getLabel()
```


시간 눈금 계층에 대한 날짜 레이블 [DateLabel](../../com.aspose.tasks/datelabel)을 가져옵니다.

**Returns:**
int - 시간 눈금 계층에 대한 날짜 레이블 [DateLabel](../../com.aspose.tasks/datelabel).
### getRenderLabelOnEachPage() {#getRenderLabelOnEachPage--}
```
public final boolean getRenderLabelOnEachPage()
```


시간 기간이 여러 페이지에 걸칠 때 각 페이지에 날짜 레이블을 렌더링할지 여부를 정의하는 플래그를 가져옵니다. 값이 'true'이면, 기간이 여러 페이지에 걸칠 때 해당 기간의 날짜 레이블이 각 페이지에 렌더링됩니다. 값이 'false'이면, `Alignment`([getAlignment](../../com.aspose.tasks/timescaletier\#getAlignment--)/[setAlignment(int)](../../com.aspose.tasks/timescaletier\#setAlignment-int-)) 속성 값에 따라 날짜 레이블이 한 번만 렌더링됩니다.

--------------------

MS Project에는 해당하는 항목이 없습니다.

**Returns:**
boolean - 기간이 여러 페이지에 걸칠 때 각 페이지에 날짜 레이블을 렌더링할지 정의하는 플래그.
### getShowTicks() {#getShowTicks--}
```
public final boolean getShowTicks()
```


계층에서 시간 기간을 구분하는 눈금 표시를 표시할지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 계층에서 시간 기간을 구분하는 눈금 표시를 보여줄지 여부를 나타내는 값.
### getUnit() {#getUnit--}
```
public final int getUnit()
```


시간 눈금 계층에 대한 timescale 단위 [TimescaleUnit](../../com.aspose.tasks/timescaleunit)를 가져옵니다. 기본값은 [TimescaleUnit](../../com.aspose.tasks/timescaleunit)입니다.

**Returns:**
int - 시간 눈금 계층에 대한 timescale 단위 [TimescaleUnit](../../com.aspose.tasks/timescaleunit).
### getUsesFiscalYear() {#getUsesFiscalYear--}
```
public final boolean getUsesFiscalYear()
```


계층 레이블을 회계 연도 기준으로 할지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 계층 레이블을 회계 연도 기준으로 할지 여부를 나타내는 값.
### setAlignment(int value) {#setAlignment-int-}
```
public final void setAlignment(int value)
```


계층의 각 시간 기간 내에서 레이블을 정렬하는 방법을 설정합니다 ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | int | 계층의 각 시간 기간 내에서 레이블을 정렬하는 방법 ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)). |

### setCount(int value) {#setCount-int-}
```
public final void setCount(int value)
```


계층에 레이블을 표시할 시간 단위 간격을 설정합니다. 기본값은 1입니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 계층에 레이블을 표시할 시간 단위 간격. |

### setDateTimeConverter(DateTimeConverter value) {#setDateTimeConverter-com.aspose.tasks.DateTimeConverter-}
```
public final void setDateTimeConverter(DateTimeConverter value)
```


이 계층에서 날짜 틱 렌더링을 처리하기 위한 콜백 함수를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [DateTimeConverter](../../com.aspose.tasks/datetimeconverter) | 이 계층에서 날짜 눈금 렌더링을 처리하기 위한 콜백 함수. |

### setLabel(int value) {#setLabel-int-}
```
public final void setLabel(int value)
```


시간 눈금 계층에 대한 날짜 레이블 [DateLabel](../../com.aspose.tasks/datelabel)를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | int | 시간 눈금 계층에 대한 날짜 레이블 [DateLabel](../../com.aspose.tasks/datelabel). |

### setRenderLabelOnEachPage(boolean value) {#setRenderLabelOnEachPage-boolean-}
```
public final void setRenderLabelOnEachPage(boolean value)
```


기간이 여러 페이지에 걸칠 때 각 페이지에 날짜 레이블을 렌더링할지 정의하는 플래그를 설정합니다. 값이 'true'이면 기간이 여러 페이지에 걸칠 때 해당 기간의 날짜 레이블이 각 페이지에 렌더링됩니다. 값이 'false'이면 `Alignment`([getAlignment](../../com.aspose.tasks/timescaletier\#getAlignment--)/[setAlignment(int)](../../com.aspose.tasks/timescaletier\#setAlignment-int-)) 속성값에 따라 날짜 레이블이 한 번만 렌더링됩니다.

--------------------

MS Project에는 해당하는 항목이 없습니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 기간이 여러 페이지에 걸칠 때 각 페이지에 날짜 레이블을 렌더링할지 정의하는 플래그. |

### setShowTicks(boolean value) {#setShowTicks-boolean-}
```
public final void setShowTicks(boolean value)
```


계층에서 시간 기간을 구분하는 눈금 표시를 표시할지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 계층에서 시간 기간을 구분하는 눈금 표시를 보여줄지 여부를 나타내는 값. |

### setUnit(int value) {#setUnit-int-}
```
public final void setUnit(int value)
```


시간 눈금 계층에 대한 timescale 단위 [TimescaleUnit](../../com.aspose.tasks/timescaleunit)를 설정합니다. 기본값은 [TimescaleUnit](../../com.aspose.tasks/timescaleunit)입니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | int | 시간 눈금 계층에 대한 timescale 단위 [TimescaleUnit](../../com.aspose.tasks/timescaleunit). |

### setUsesFiscalYear(boolean value) {#setUsesFiscalYear-boolean-}
```
public final void setUsesFiscalYear(boolean value)
```


계층 레이블을 회계 연도 기준으로 할지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 계층 레이블을 회계 연도 기준으로 할지 여부를 나타내는 값. |

