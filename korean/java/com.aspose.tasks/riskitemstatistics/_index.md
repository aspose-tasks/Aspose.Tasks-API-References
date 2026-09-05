---
title: "RiskItemStatistics"
second_title: "Aspose.Tasks for Java API Reference"
description: "분석된 프로젝트의 작업에 대한 통계 데이터를 저장하는 항목을 나타냅니다."
type: docs
weight: 265
url: /ko/java/com.aspose.tasks/riskitemstatistics/
---

**Inheritance:**
java.lang.Object
```
public class RiskItemStatistics
```

분석된 프로젝트의 작업에 대한 통계 데이터를 저장하는 항목을 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getExpectedValue()](#getExpectedValue--) | 위험 항목의 기대값을 가져옵니다. |
| [getItemType()](#getItemType--) | [RiskItemType](../../com.aspose.tasks/riskitemtype) 열거형의 인스턴스를 가져옵니다. |
| [getMaximum()](#getMaximum--) | 몬테카를로 시뮬레이션 중에 생성된 최대값을 가져옵니다. |
| [getMinimum()](#getMinimum--) | 몬테카를로 시뮬레이션 중에 생성된 최소값을 가져옵니다. |
| [getPercentile(int percent)](#getPercentile-int-) | 생성된 샘플 중 지정된 백분율이 이하가 되는 값을 가져옵니다. |
| [getStandardDeviation()](#getStandardDeviation--) | 위험 항목의 표준 편차를 가져옵니다. |
| [toString()](#toString--) | 위험 항목의 짧은 문자열 표현을 반환합니다. |
### getExpectedValue() {#getExpectedValue--}
```
public final Date getExpectedValue()
```


위험 항목의 기대값을 가져옵니다.

**Returns:**
java.util.Date - 위험 항목의 기대값.
### getItemType() {#getItemType--}
```
public final int getItemType()
```


[RiskItemType](../../com.aspose.tasks/riskitemtype) 열거형의 인스턴스를 가져옵니다.

**Returns:**
int - [RiskItemType](../../com.aspose.tasks/riskitemtype) 열거형의 인스턴스.
### getMaximum() {#getMaximum--}
```
public final Date getMaximum()
```


몬테카를로 시뮬레이션 중에 생성된 최대값을 가져옵니다.

**Returns:**
java.util.Date - 몬테카를로 시뮬레이션 중에 생성된 최대값.
### getMinimum() {#getMinimum--}
```
public final Date getMinimum()
```


몬테카를로 시뮬레이션 중에 생성된 최소값을 가져옵니다.

**Returns:**
java.util.Date - 몬테카를로 시뮬레이션 중에 생성된 최소값.
### getPercentile(int percent) {#getPercentile-int-}
```
public final Date getPercentile(int percent)
```


생성된 샘플 중 지정된 백분율이 이하가 되는 값을 가져옵니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 백분율 | int | 0과 100 사이의 지정된 백분율. |

**Returns:**
java.util.Date - 생성된 샘플 중 지정된 백분율이 이하가 되는 값.
### getStandardDeviation() {#getStandardDeviation--}
```
public final Duration getStandardDeviation()
```


위험 항목의 표준 편차를 가져옵니다.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the standard deviation of the risk item.
### toString() {#toString--}
```
public String toString()
```


위험 항목의 짧은 문자열 표현을 반환합니다. 표현의 정확한 세부 사항은 지정되지 않았으며 변경될 수 있습니다.

**Returns:**
java.lang.String - RiskItem 객체를 나타내는 짧은 문자열.
