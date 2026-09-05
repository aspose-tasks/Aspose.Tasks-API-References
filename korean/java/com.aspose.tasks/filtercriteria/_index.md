---
title: "FilterCriteria"
second_title: "Aspose.Tasks for Java API Reference"
description: "MSP 보기에서 표시되기 위해 작업 또는 리소스가 충족해야 하는 기준을 정의합니다."
type: docs
weight: 94
url: /ko/java/com.aspose.tasks/filtercriteria/
---

**Inheritance:**
java.lang.Object
```
public class FilterCriteria
```

MSP 보기에서 표시되기 위해 작업 또는 리소스가 충족해야 하는 기준을 정의합니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [FilterCriteria()](#FilterCriteria--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getCriteriaRows()](#getCriteriaRows--) | 자식 [FilterCriteria](../../com.aspose.tasks/filtercriteria) 행의 목록을 가져옵니다. |
| [getField()](#getField--) | 변경할 `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-))를 가져옵니다. |
| [getOperation()](#getOperation--) | FieldName, Test 및 Value로 설정된 기준이 필터의 다른 기준과 어떻게 관련되는지 가져옵니다. |
| [getTest()](#getTest--) | 필터의 선택 기준으로 작용하는 FieldName과 Value 사이의 비교 유형을 가져옵니다. |
| [getValues()](#getValues--) | FieldName으로 지정된 필드의 값과 비교할 객체 값을 가져옵니다. |
| [isValueAField()](#isValueAField--) | FilterCriteria의 오른쪽 값이 상수가 아닌 필드 참조인지 여부를 가져옵니다. |
| [isValueAField(int index)](#isValueAField-int-) | FilterCriteria 인덱스에 있는 값이 상수가 아닌 필드 참조인지 여부를 가져옵니다. |
| [setField(int value)](#setField-int-) | 변경할 `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-))를 설정합니다. |
| [setOperation(int value)](#setOperation-int-) | 필터에서 FieldName, Test 및 Value 로 설정된 기준이 다른 기준과 관련됩니다. |
| [setTest(int value)](#setTest-int-) | 필터의 선택 기준으로 작용하는 FieldName과 Value 사이의 비교 유형을 설정합니다. |
| [setValue(int index, Object value)](#setValue-int-java.lang.Object-) | FieldName으로 지정된 필드의 값과 비교하기 위해 인덱스에 있는 객체 값을 설정합니다. |
| [setValue(Object value)](#setValue-java.lang.Object-) | FieldName으로 지정된 필드의 값과 비교할 객체 값을 설정합니다. |
| [setValueByField(int value)](#setValueByField-int-) | FieldName으로 지정된 필드의 값과 비교될 값의 필드를 설정합니다. |
| [setValueByField(int index, int value)](#setValueByField-int-int-) | FieldName으로 지정된 필드의 값과 비교될 값의 필드를 인덱스에 설정합니다. |
| [toString()](#toString--) | [FilterCriteria](../../com.aspose.tasks/filtercriteria) 클래스 인스턴스의 문자열 표현을 반환합니다. |
### FilterCriteria() {#FilterCriteria--}
```
public FilterCriteria()
```


### getCriteriaRows() {#getCriteriaRows--}
```
public final List<FilterCriteria> getCriteriaRows()
```


자식 [FilterCriteria](../../com.aspose.tasks/filtercriteria) 행 목록을 가져옵니다. 필터에 하나 이상의 기준 행이 포함된 경우 And 연산자의 효과는 두 행의 기준이 모두 충족되어야 해당 작업이나 리소스가 이 필터의 결과로 표시된다는 것입니다. Or 연산자의 효과는 두 행 중 하나의 기준만 충족되면 된다는 것입니다.

**Returns:**
java.util.List&lt;com.aspose.tasks.FilterCriteria&gt; - 자식 [FilterCriteria](../../com.aspose.tasks/filtercriteria) 행 목록입니다.
### getField() {#getField--}
```
public final int getField()
```


변경할 `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-))를 가져옵니다.

**Returns:**
int - 변경할 `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) 입니다.
### getOperation() {#getOperation--}
```
public final int getOperation()
```


FieldName, Test 및 Value로 설정된 기준이 필터의 다른 기준과 어떻게 관련되는지 가져옵니다.

**Returns:**
int - 필터에서 FieldName, Test 및 Value 로 설정된 기준이 다른 기준과 관련됩니다.
### getTest() {#getTest--}
```
public final int getTest()
```


필터의 선택 기준으로 작용하는 FieldName과 Value 사이의 비교 유형을 가져옵니다. [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Returns:**
int - 필터의 선택 기준으로 작용하는 FieldName과 Value 사이의 비교 유형입니다.
### getValues() {#getValues--}
```
public final Object[] getValues()
```


FieldName으로 지정된 필드의 값과 비교할 객체 값을 가져옵니다.

**Returns:**
java.lang.Object[] - FieldName으로 지정된 필드의 값과 비교할 객체 값들입니다.
### isValueAField() {#isValueAField--}
```
public final boolean isValueAField()
```


FilterCriteria의 오른쪽 값이 상수가 아닌 필드 참조인지 여부를 가져옵니다.

**Returns:**
boolean - FilterCriteria의 오른쪽 값이 상수가 아닌 필드 참조인지 여부입니다.
### isValueAField(int index) {#isValueAField-int-}
```
public final boolean isValueAField(int index)
```


FilterCriteria 인덱스에 있는 값이 상수가 아닌 필드 참조인지 여부를 가져옵니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| index | int | 값의 인덱스 |

**Returns:**
boolean - FilterCriteria 인덱스의 오른쪽 값이 상수가 아닌 필드 참조인지 여부입니다.
### setField(int value) {#setField-int-}
```
public final void setField(int value)
```


변경할 `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-))를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | int | `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) 를 변경합니다. |

### setOperation(int value) {#setOperation-int-}
```
public final void setOperation(int value)
```


필터에서 FieldName, Test 및 Value 로 설정된 기준이 다른 기준과 관련됩니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | FieldName, Test 및 Value 로 설정된 기준이 필터의 다른 기준과 관련됩니다. |

### setTest(int value) {#setTest-int-}
```
public final void setTest(int value)
```


필터의 선택 기준으로 작용하는 FieldName과 Value 사이의 비교 유형을 설정합니다. [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 필터의 선택 기준으로 작용하는 FieldName과 Value 사이의 비교 유형. |

### setValue(int index, Object value) {#setValue-int-java.lang.Object-}
```
public final void setValue(int index, Object value)
```


FieldName으로 지정된 필드의 값과 비교하기 위해 인덱스에 있는 객체 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| index | int | 값의 인덱스. |
| 값 | java.lang.Object | 필터 기준 인덱스에서 오른쪽 값으로 사용될 객체 값. |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public final void setValue(Object value)
```


FieldName으로 지정된 필드의 값과 비교할 객체 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.Object | 필터 기준의 오른쪽 값으로 사용될 객체 값. |

### setValueByField(int value) {#setValueByField-int-}
```
public final void setValueByField(int value)
```


FieldName으로 지정된 필드의 값과 비교될 값의 필드를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 필터 기준의 오른쪽 값으로 사용될 필드. |

### setValueByField(int index, int value) {#setValueByField-int-int-}
```
public final void setValueByField(int index, int value)
```


FieldName으로 지정된 필드의 값과 비교될 값의 필드를 인덱스에 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| index | int | 값의 인덱스 |
| 값 | int | 필터 기준의 인덱스에서 오른쪽 값으로 사용되는 필드입니다. |

### toString() {#toString--}
```
public String toString()
```


[FilterCriteria](../../com.aspose.tasks/filtercriteria) 클래스 인스턴스의 문자열 표현을 반환합니다.

**Returns:**
java.lang.String - 이 객체의 문자열 표현.
