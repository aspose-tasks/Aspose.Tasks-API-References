---
title: "비율."
second_title: "Aspose.Tasks for Java API Reference"
description: "해당 기간 동안 리소스에 적용되는 시간 기간 및 요금 정의를 나타냅니다."
type: docs
weight: 232
url: /ko/java/com.aspose.tasks/rate/
---

**Inheritance:**
java.lang.Object
```
public class Rate
```

해당 기간 동안 리소스에 적용되는 시간 기간 및 요금 정의를 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getCostPerUse()](#getCostPerUse--) | 리소스 사용당 비용을 가져옵니다. |
| [getOvertimeRate()](#getOvertimeRate--) | 리소스의 시간당 초과근무 요금을 가져옵니다. |
| [getOvertimeRateFormat()](#getOvertimeRateFormat--) | Microsoft Project에서 초과근무 요금을 표시하는 데 사용되는 단위를 가져옵니다. |
| [getRateTable()](#getRateTable--) | 리소스에 대한 요금표의 고유 식별자를 가져옵니다. |
| [getRatesFrom()](#getRatesFrom--) | 요금이 적용되는 날짜를 가져옵니다. |
| [getRatesTo()](#getRatesTo--) | 요금이 유효한 마지막 날짜를 가져옵니다. |
| [getStandardRate()](#getStandardRate--) | 리소스의 시간당 표준 요금을 가져옵니다. |
| [getStandardRateFormat()](#getStandardRateFormat--) | Microsoft Project에서 표준 요금을 표시하는 데 사용되는 단위를 가져옵니다. |
| [setCostPerUse(BigDecimal value)](#setCostPerUse-java.math.BigDecimal-) | 리소스 사용당 비용을 설정합니다. |
| [setOvertimeRate(BigDecimal value)](#setOvertimeRate-java.math.BigDecimal-) | 리소스의 시간당 초과 근무 요금을 설정합니다. |
| [setOvertimeRateFormat(int value)](#setOvertimeRateFormat-int-) | Microsoft Project에서 초과 근무 요금을 표시하는 데 사용되는 단위를 설정합니다. |
| [setRateTable(int value)](#setRateTable-int-) | 리소스에 대한 요금표의 고유 식별자를 설정합니다. |
| [setRatesFrom(Date value)](#setRatesFrom-java.util.Date-) | 요금이 적용되는 날짜를 설정합니다. |
| [setRatesTo(Date value)](#setRatesTo-java.util.Date-) | 요금이 유효한 마지막 날짜를 설정합니다. |
| [setStandardRate(BigDecimal value)](#setStandardRate-java.math.BigDecimal-) | 리소스의 시간당 표준 요금을 설정합니다. |
| [setStandardRateFormat(int value)](#setStandardRateFormat-int-) | Microsoft Project에서 표준 요금을 표시하는 데 사용되는 단위를 설정합니다. |
### getCostPerUse() {#getCostPerUse--}
```
public final BigDecimal getCostPerUse()
```


리소스 사용당 비용을 가져옵니다. 요금표가 리소스에 존재하는 경우 현재 날짜에서 이 값을 검색합니다.

**Returns:**
java.math.BigDecimal - 리소스 사용당 비용.
### getOvertimeRate() {#getOvertimeRate--}
```
public final BigDecimal getOvertimeRate()
```


리소스의 시간당 초과근무 요금을 가져옵니다.

**Returns:**
java.math.BigDecimal - 리소스의 시간당 초과 근무 요금.
### getOvertimeRateFormat() {#getOvertimeRateFormat--}
```
public final int getOvertimeRateFormat()
```


Microsoft Project에서 초과근무 요금을 표시하는 데 사용되는 단위를 가져옵니다.

**Returns:**
int - Microsoft Project에서 초과 근무 요금을 표시하는 데 사용되는 단위.
### getRateTable() {#getRateTable--}
```
public final int getRateTable()
```


리소스에 대한 요금표의 고유 식별자를 가져옵니다.

**Returns:**
int - 리소스에 대한 요금표의 고유 식별자.
### getRatesFrom() {#getRatesFrom--}
```
public final Date getRatesFrom()
```


요금이 적용되는 날짜를 가져옵니다.

**Returns:**
java.util.Date - 요금이 적용되는 날짜.
### getRatesTo() {#getRatesTo--}
```
public final Date getRatesTo()
```


요금이 유효한 마지막 날짜를 가져옵니다.

**Returns:**
java.util.Date - 요금이 유효한 마지막 날짜.
### getStandardRate() {#getStandardRate--}
```
public final BigDecimal getStandardRate()
```


리소스의 시간당 표준 요금을 가져옵니다.

**Returns:**
java.math.BigDecimal - 리소스의 시간당 표준 요금.
### getStandardRateFormat() {#getStandardRateFormat--}
```
public final int getStandardRateFormat()
```


Microsoft Project에서 표준 요금을 표시하는 데 사용되는 단위를 가져옵니다.

**Returns:**
int - Microsoft Project에서 표준 요금을 표시하는 데 사용되는 단위.
### setCostPerUse(BigDecimal value) {#setCostPerUse-java.math.BigDecimal-}
```
public final void setCostPerUse(BigDecimal value)
```


리소스 사용당 비용을 설정합니다. 요금표가 리소스에 존재하는 경우 현재 날짜에서 이 값을 검색합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.math.BigDecimal | 리소스 사용당 비용. |

### setOvertimeRate(BigDecimal value) {#setOvertimeRate-java.math.BigDecimal-}
```
public final void setOvertimeRate(BigDecimal value)
```


리소스의 시간당 초과 근무 요금을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.math.BigDecimal | 리소스의 시간당 초과 근무 요금. |

### setOvertimeRateFormat(int value) {#setOvertimeRateFormat-int-}
```
public final void setOvertimeRateFormat(int value)
```


Microsoft Project에서 초과 근무 요금을 표시하는 데 사용되는 단위를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | Microsoft Project에서 초과 근무 요금을 표시하는 데 사용되는 단위. |

### setRateTable(int value) {#setRateTable-int-}
```
public final void setRateTable(int value)
```


리소스에 대한 요금표의 고유 식별자를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 리소스에 대한 요금표의 고유 식별자. |

### setRatesFrom(Date value) {#setRatesFrom-java.util.Date-}
```
public final void setRatesFrom(Date value)
```


요금이 적용되는 날짜를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date | 요금이 적용되는 날짜. |

### setRatesTo(Date value) {#setRatesTo-java.util.Date-}
```
public final void setRatesTo(Date value)
```


요금이 유효한 마지막 날짜를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date | 요금이 유효한 마지막 날짜. |

### setStandardRate(BigDecimal value) {#setStandardRate-java.math.BigDecimal-}
```
public final void setStandardRate(BigDecimal value)
```


리소스의 시간당 표준 요금을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.math.BigDecimal | 리소스의 시간당 표준 요금. |

### setStandardRateFormat(int value) {#setStandardRateFormat-int-}
```
public final void setStandardRateFormat(int value)
```


Microsoft Project에서 표준 요금을 표시하는 데 사용되는 단위를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | Microsoft Project에서 표준 요금을 표시하는 데 사용되는 단위. |

