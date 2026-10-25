---
title: "GraphicalIndicatorCriteria"
second_title: "Aspose.Tasks for Java API Reference"
description: "확장 속성과 연결된 하나의 그래픽 지표 기준을 나타냅니다."
type: docs
weight: 115
url: /ko/java/com.aspose.tasks/graphicalindicatorcriteria/
---

**Inheritance:**
java.lang.Object
```
public final class GraphicalIndicatorCriteria
```

확장 속성과 연결된 하나의 그래픽 지표 기준을 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2)](#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-com.aspose.tasks.GraphicalIndicatorCriteriaValue-) | 새 인스턴스를 초기화합니다 [GraphicalIndicatorCriteria](../../com.aspose/tasks/graphicalindicatorcriteria) 유형을. |
| [GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value)](#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-) | 새 인스턴스를 초기화합니다 [GraphicalIndicatorCriteria](../../com.aspose/tasks/graphicalindicatorcriteria) 유형을. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getImageIndex()](#getImageIndex--) | 필드가 기준을 충족할 때 표시할 이미지의 인덱스를 가져옵니다. |
| [getRowType()](#getRowType--) | [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) 열거형의 값을 가져옵니다. 이 열거형은 인디케이터가 적용되는 행을 나타냅니다. |
| [getTest()](#getTest--) | 확장 속성 값과 값 사이의 비교 유형을 가져옵니다. 이는 그래픽 인디케이터 적용 기준으로 작동합니다. |
| [getValue1()](#getValue1--) | 확장 속성 값을 테스트하는 데 사용되는 값을 가져옵니다. |
| [getValue2()](#getValue2--) | 'IsWithin' 및 'IsNotWithin' 비교 유형인 경우 확장 속성 값을 테스트하는 데 사용되는 두 번째 값을 가져옵니다. |
| [toString()](#toString--) | [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria) 클래스 인스턴스의 문자열 표현을 반환합니다. |
### GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2) {#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-com.aspose.tasks.GraphicalIndicatorCriteriaValue-}
```
public GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2)
```


새 인스턴스를 초기화합니다 [GraphicalIndicatorCriteria](../../com.aspose/tasks/graphicalindicatorcriteria) 유형을.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| rowType | int | [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) 열거형 값으로, 인디케이터가 적용되는 행을 나타냅니다 |
| test | int | [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype) 값으로, 기준에 의해 수행되는 비교 유형을 나타냅니다. |
| imageIndex | int | 필드가 기준을 충족할 때 표시할 이미지의 인덱스 |
| value1 | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | 조건 검사에 사용되는 값들. |
| value2 | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | 'IsWithin' 및 'IsNotWithing' 조건인 경우 조건 검사에 사용되는 두 번째 값(구간 끝)입니다. |

### GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value) {#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-}
```
public GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value)
```


새 인스턴스를 초기화합니다 [GraphicalIndicatorCriteria](../../com.aspose/tasks/graphicalindicatorcriteria) 유형을.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| rowType | int | [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) 열거형 값으로, 인디케이터가 적용되는 행을 나타냅니다 |
| test | int | [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype) 값으로, 기준에 의해 수행되는 비교 유형을 나타냅니다. |
| imageIndex | int | 필드가 기준을 충족할 때 표시할 이미지의 인덱스 |
| value | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | 조건 검사에 사용되는 값. |

### getImageIndex() {#getImageIndex--}
```
public final int getImageIndex()
```


필드가 기준을 충족할 때 표시할 이미지의 인덱스를 가져옵니다.

**Returns:**
int - 필드가 기준을 충족할 때 표시할 이미지의 인덱스.
### getRowType() {#getRowType--}
```
public final int getRowType()
```


[GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) 열거형의 값을 가져옵니다. 이 열거형은 인디케이터가 적용되는 행을 나타냅니다.

**Returns:**
int - 인디케이터가 적용되는 행을 나타내는 [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) 열거형 값.
### getTest() {#getTest--}
```
public final int getTest()
```


확장 속성 값과 값 사이의 비교 유형을 가져옵니다. 이는 그래픽 인디케이터 적용 기준으로 작동합니다. [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Returns:**
int - 확장 속성 값과 값 사이의 비교 유형으로, 그래픽 인디케이터 적용 기준으로 작동합니다.
### getValue1() {#getValue1--}
```
public final GraphicalIndicatorCriteriaValue getValue1()
```


확장 속성 값을 테스트하는 데 사용되는 값을 가져옵니다.

**Returns:**
[GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) - the value used to test extended attribute's value.
### getValue2() {#getValue2--}
```
public final GraphicalIndicatorCriteriaValue getValue2()
```


'IsWithin' 및 'IsNotWithin' 비교 유형인 경우 확장 속성 값을 테스트하는 데 사용되는 두 번째 값을 가져옵니다.

**Returns:**
[GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) - the second value used to test extended attribute's value in case of 'IsWithin' and 'IsNotWithin' comparison types.
### toString() {#toString--}
```
public String toString()
```


[GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria) 클래스 인스턴스의 문자열 표현을 반환합니다.

**Returns:**
java.lang.String - 이 객체의 문자열 표현.
