---
title: "GraphicalIndicatorCriteriaValue"
second_title: "Aspose.Tasks for Java API Reference"
description: "그래픽 지표 기준의 조건 검사에 사용되는 값을 나타냅니다."
type: docs
weight: 117
url: /ko/java/com.aspose.tasks/graphicalindicatorcriteriavalue/
---

**Inheritance:**
java.lang.Object
```
public final class GraphicalIndicatorCriteriaValue
```

그래픽 지표 기준의 조건 검사에 사용되는 값을 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [GraphicalIndicatorCriteriaValue(BigDecimal value)](#GraphicalIndicatorCriteriaValue-java.math.BigDecimal-) | GraphicalIndicatorCriteriaValue 클래스의 인스턴스를 상수 BigDecimal 값으로 생성합니다. |
| [GraphicalIndicatorCriteriaValue(Date dateValue)](#GraphicalIndicatorCriteriaValue-java.util.Date-) | GraphicalIndicatorCriteriaValue 클래스의 인스턴스를 상수 Date 값으로 생성합니다. |
| [GraphicalIndicatorCriteriaValue(String textValue)](#GraphicalIndicatorCriteriaValue-java.lang.String-) | GraphicalIndicatorCriteriaValue 클래스의 인스턴스를 상수 String 값으로 생성합니다. |
| [GraphicalIndicatorCriteriaValue(Duration durationValue)](#GraphicalIndicatorCriteriaValue-com.aspose.tasks.Duration-) | GraphicalIndicatorCriteriaValue 클래스의 인스턴스를 상수 Duration 값으로 생성합니다. |
| [GraphicalIndicatorCriteriaValue(boolean flagValue)](#GraphicalIndicatorCriteriaValue-boolean-) | GraphicalIndicatorCriteriaValue 클래스의 인스턴스를 상수 flag (boolean) 값으로 생성합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [createFieldLink(int field)](#createFieldLink-int-) | GraphicalIndicatorCriteriaValue 클래스의 인스턴스를 지정된 MS Project 필드의 값을 나타내도록 생성합니다. |
| [getRawValue()](#getRawValue--) | Field 값의 기본 상수를 가져옵니다. |
| [isFieldLink()](#isFieldLink--) | 현재 인스턴스가 필드 링크인지(필드 값을 나타내는지) 여부를 가져옵니다. |
| [toString()](#toString--) | 현재 객체를 나타내는 문자열을 반환합니다. |
### GraphicalIndicatorCriteriaValue(BigDecimal value) {#GraphicalIndicatorCriteriaValue-java.math.BigDecimal-}
```
public GraphicalIndicatorCriteriaValue(BigDecimal value)
```


GraphicalIndicatorCriteriaValue 클래스의 인스턴스를 상수 BigDecimal 값으로 생성합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.math.BigDecimal | BigDecimal 값 |

### GraphicalIndicatorCriteriaValue(Date dateValue) {#GraphicalIndicatorCriteriaValue-java.util.Date-}
```
public GraphicalIndicatorCriteriaValue(Date dateValue)
```


GraphicalIndicatorCriteriaValue 클래스의 인스턴스를 상수 Date 값으로 생성합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| dateValue | java.util.Date | Date 값 |

### GraphicalIndicatorCriteriaValue(String textValue) {#GraphicalIndicatorCriteriaValue-java.lang.String-}
```
public GraphicalIndicatorCriteriaValue(String textValue)
```


GraphicalIndicatorCriteriaValue 클래스의 인스턴스를 상수 String 값으로 생성합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| textValue | java.lang.String | String 값 |

### GraphicalIndicatorCriteriaValue(Duration durationValue) {#GraphicalIndicatorCriteriaValue-com.aspose.tasks.Duration-}
```
public GraphicalIndicatorCriteriaValue(Duration durationValue)
```


GraphicalIndicatorCriteriaValue 클래스의 인스턴스를 상수 Duration 값으로 생성합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| durationValue | [Duration](../../com.aspose.tasks/duration) | Duration 값 |

### GraphicalIndicatorCriteriaValue(boolean flagValue) {#GraphicalIndicatorCriteriaValue-boolean-}
```
public GraphicalIndicatorCriteriaValue(boolean flagValue)
```


GraphicalIndicatorCriteriaValue 클래스의 인스턴스를 상수 flag (boolean) 값으로 생성합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| flagValue | boolean | flag (boolean) 값 |

### createFieldLink(int field) {#createFieldLink-int-}
```
public static GraphicalIndicatorCriteriaValue createFieldLink(int field)
```


GraphicalIndicatorCriteriaValue 클래스의 인스턴스를 지정된 MS Project 필드의 값을 나타내도록 생성합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 필드 | int | 지정된 필드 |

**Returns:**
[GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) - instance of GraphicalIndicatorCriteriaValue class representing the value of the specified field
### getRawValue() {#getRawValue--}
```
public final Object getRawValue()
```


Field 값의 기본 상수를 가져옵니다.

**Returns:**
java.lang.Object - Field 값의 기본 상수
### isFieldLink() {#isFieldLink--}
```
public final boolean isFieldLink()
```


현재 인스턴스가 필드 링크인지(필드 값을 나타내는지) 여부를 가져옵니다.

**Returns:**
boolean - 현재 인스턴스가 필드 링크인지(필드 값을 나타내는지) 여부
### toString() {#toString--}
```
public String toString()
```


현재 객체를 나타내는 문자열을 반환합니다.

**Returns:**
java.lang.String - 현재 객체를 나타내는 문자열
