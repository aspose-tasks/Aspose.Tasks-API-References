---
title: "Filter"
second_title: "Aspose.Tasks for Java API Reference"
description: "프로젝트의 필터를 나타냅니다."
type: docs
weight: 91
url: /ko/java/com.aspose.tasks/filter/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable, com.aspose.ms.System.IEquatable
```
public final class Filter implements Comparable<Filter>, System.IEquatable<Filter>
```

프로젝트의 필터를 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [Filter()](#Filter--) |  |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [compareTo(Filter other)](#compareTo-com.aspose.tasks.Filter-) | 이 인스턴스를 [Filter](../../com.aspose.tasks/filter) 클래스의 지정된 인스턴스와 비교하고, 상대적인 순서를 나타내는 값을 반환합니다. |
| [equals(Filter other)](#equals-com.aspose.tasks.Filter-) | 이 인스턴스가 지정된 AssignmentBaseline 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| [equals(Object obj)](#equals-java.lang.Object-) | 이 인스턴스가 지정된 AssignmentBaseline 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| [getCriteria()](#getCriteria--) | MSP 보기에서 표시되기 위해 작업 또는 리소스가 충족해야 하는 기준을 가져옵니다. |
| [getFilterType()](#getFilterType--) | 필터의 유형을 가져옵니다. |
| [getIndex()](#getIndex--) | Filters 포함 객체에서 [Filter](../../com.aspose.tasks/filter) 객체의 인덱스를 가져옵니다. |
| [getName()](#getName--) | Filter 객체의 이름을 가져옵니다. |
| [getShowInMenu()](#getShowInMenu--) | 프로젝트가 리본의 View 탭에 있는 Filter 드롭다운 목록에 필터 이름을 표시하는지 여부를 나타내는 값을 가져옵니다. |
| [getShowRelatedSummaryRows()](#getShowRelatedSummaryRows--) | 필터에 대해 관련 요약 행이 표시되는지 여부를 나타내는 값을 가져옵니다. |
| [getUid()](#getUid--) | 필터의 고유 식별자를 가져옵니다. |
| [hashCode()](#hashCode--) | 필터에 대한 해시 코드 값을 반환합니다. |
| [op_Equality(Filter a, Filter b)](#op-Equality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| [op_GreaterThan(Filter a, Filter b)](#op-GreaterThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | 이 인스턴스가 지정된 객체보다 큰지 여부를 나타내는 값을 반환합니다. |
| [op_GreaterThanOrEqual(Filter a, Filter b)](#op-GreaterThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | 이 인스턴스가 지정된 객체보다 크거나 같은지 여부를 나타내는 값을 반환합니다. |
| [op_Inequality(Filter a, Filter b)](#op-Inequality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | 이 인스턴스가 지정된 객체와 같지 않은지 여부를 나타내는 값을 반환합니다. |
| [op_LessThan(Filter a, Filter b)](#op-LessThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | 이 인스턴스가 지정된 객체보다 작은지 여부를 나타내는 값을 반환합니다. |
| [op_LessThanOrEqual(Filter a, Filter b)](#op-LessThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | 이 인스턴스가 지정된 객체보다 작거나 같은지 여부를 나타내는 값을 반환합니다. |
| [setCriteria(FilterCriteria value)](#setCriteria-com.aspose.tasks.FilterCriteria-) | MSP 보기에서 표시되기 위해 작업 또는 리소스가 충족해야 하는 기준을 설정합니다. |
| [setFilterType(int value)](#setFilterType-int-) | 필터의 유형입니다. |
| [setName(String value)](#setName-java.lang.String-) | Filter 객체의 이름을 설정합니다. |
| [setShowInMenu(boolean value)](#setShowInMenu-boolean-) | 프로젝트가 리본의 View 탭에 있는 Filter 드롭다운 목록에 필터 이름을 표시하는지 여부를 나타내는 값을 설정합니다. |
| [setShowRelatedSummaryRows(boolean value)](#setShowRelatedSummaryRows-boolean-) | 필터에 대해 관련 요약 행이 표시되는지 여부를 나타내는 값을 설정합니다. |
### Filter() {#Filter--}
```
public Filter()
```


### compareTo(Filter other) {#compareTo-com.aspose.tasks.Filter-}
```
public final int compareTo(Filter other)
```


이 인스턴스를 [Filter](../../com.aspose.tasks/filter) 클래스의 지정된 인스턴스와 비교하고, 상대적인 순서를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| other | [Filter](../../com.aspose.tasks/filter) | 이 객체와 비교할 지정된 [Filter](../../com.aspose.tasks/filter) 클래스 인스턴스. |

**Returns:**
int - 상대 순서를 나타내는 표시.
### equals(Filter other) {#equals-com.aspose.tasks.Filter-}
```
public final boolean equals(Filter other)
```


이 인스턴스가 지정된 AssignmentBaseline 객체와 같은지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| other | [Filter](../../com.aspose.tasks/filter) | 이 인스턴스와 비교할 지정된 AssignmentBaseline 객체. |

**Returns:**
boolean - 이 인스턴스가 지정된 AssignmentBaseline 객체와 같으면 true를 반환하고, 그렇지 않으면 false를 반환합니다.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


이 인스턴스가 지정된 AssignmentBaseline 객체와 같은지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| obj | java.lang.Object | 이 인스턴스와 비교할 지정된 AssignmentBaseline 객체. |

**Returns:**
boolean - 이 인스턴스가 지정된 AssignmentBaseline 객체와 같으면 true를 반환하고, 그렇지 않으면 false를 반환합니다.
### getCriteria() {#getCriteria--}
```
public final FilterCriteria getCriteria()
```


MSP 보기에서 표시되기 위해 작업 또는 리소스가 충족해야 하는 기준을 가져옵니다.

**Returns:**
[FilterCriteria](../../com.aspose.tasks/filtercriteria) - the criteria that tasks or resources must meet to be displayed in MSP view.
### getFilterType() {#getFilterType--}
```
public final int getFilterType()
```


필터의 유형을 가져옵니다.

**Returns:**
int - 필터의 유형.
### getIndex() {#getIndex--}
```
public final int getIndex()
```


Filters 포함 객체에서 [Filter](../../com.aspose.tasks/filter) 객체의 인덱스를 가져옵니다.

**Returns:**
int - Filters 포함 객체에서 [Filter](../../com.aspose.tasks/filter) 객체의 인덱스.
### getName() {#getName--}
```
public final String getName()
```


Filter 객체의 이름을 가져옵니다.

**Returns:**
java.lang.String - Filter 객체의 이름.
### getShowInMenu() {#getShowInMenu--}
```
public final boolean getShowInMenu()
```


프로젝트가 리본의 View 탭에 있는 Filter 드롭다운 목록에 필터 이름을 표시하는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 프로젝트가 리본의 보기 탭에 있는 필터 드롭다운 목록에 필터 이름을 표시하는지 여부를 나타내는 값.
### getShowRelatedSummaryRows() {#getShowRelatedSummaryRows--}
```
public final boolean getShowRelatedSummaryRows()
```


필터에 대해 관련 요약 행이 표시되는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 필터에 대해 관련 요약 행이 표시되는지 여부를 나타내는 값.
### getUid() {#getUid--}
```
public final int getUid()
```


필터의 고유 식별자를 가져옵니다.

**Returns:**
int - 필터의 고유 식별자.
### hashCode() {#hashCode--}
```
public int hashCode()
```


필터에 대한 해시 코드 값을 반환합니다.

**Returns:**
int - 이 객체에 대한 해시 코드 값을 반환합니다.
### op_Equality(Filter a, Filter b) {#op-Equality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_Equality(Filter a, Filter b)
```


이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | 첫 번째 필터. |
| b | [Filter](../../com.aspose.tasks/filter) | 두 번째 필터. |

**Returns:**
boolean - 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값
### op_GreaterThan(Filter a, Filter b) {#op-GreaterThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_GreaterThan(Filter a, Filter b)
```


이 인스턴스가 지정된 객체보다 큰지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | 첫 번째 필터. |
| b | [Filter](../../com.aspose.tasks/filter) | 두 번째 필터. |

**Returns:**
boolean - 이 인스턴스가 지정된 객체보다 큰지 여부를 나타내는 값
### op_GreaterThanOrEqual(Filter a, Filter b) {#op-GreaterThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_GreaterThanOrEqual(Filter a, Filter b)
```


이 인스턴스가 지정된 객체보다 크거나 같은지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | 첫 번째 필터. |
| b | [Filter](../../com.aspose.tasks/filter) | 두 번째 필터. |

**Returns:**
boolean - 이 인스턴스가 지정된 객체보다 크거나 같은지 여부를 나타내는 값
### op_Inequality(Filter a, Filter b) {#op-Inequality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_Inequality(Filter a, Filter b)
```


이 인스턴스가 지정된 객체와 같지 않은지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | 첫 번째 필터. |
| b | [Filter](../../com.aspose.tasks/filter) | 두 번째 필터. |

**Returns:**
boolean - 이 인스턴스가 지정된 객체와 같지 않은지 여부를 나타내는 값
### op_LessThan(Filter a, Filter b) {#op-LessThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_LessThan(Filter a, Filter b)
```


이 인스턴스가 지정된 객체보다 작은지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | 첫 번째 필터. |
| b | [Filter](../../com.aspose.tasks/filter) | 두 번째 필터. |

**Returns:**
boolean - 이 인스턴스가 지정된 객체보다 작은지 여부를 나타내는 값
### op_LessThanOrEqual(Filter a, Filter b) {#op-LessThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_LessThanOrEqual(Filter a, Filter b)
```


이 인스턴스가 지정된 객체보다 작거나 같은지 여부를 나타내는 값을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | 첫 번째 필터. |
| b | [Filter](../../com.aspose.tasks/filter) | 두 번째 필터. |

**Returns:**
boolean - 이 인스턴스가 지정된 객체보다 작거나 같은지 여부를 나타내는 값
### setCriteria(FilterCriteria value) {#setCriteria-com.aspose.tasks.FilterCriteria-}
```
public final void setCriteria(FilterCriteria value)
```


MSP 보기에서 표시되기 위해 작업 또는 리소스가 충족해야 하는 기준을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| value | [FilterCriteria](../../com.aspose.tasks/filtercriteria) | MSP 보기에서 표시되기 위해 작업 또는 리소스가 충족해야 하는 기준. |

### setFilterType(int value) {#setFilterType-int-}
```
public final void setFilterType(int value)
```


필터의 유형입니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | int | 필터의 유형. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Filter 객체의 이름을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | Filter 객체의 이름. |

### setShowInMenu(boolean value) {#setShowInMenu-boolean-}
```
public final void setShowInMenu(boolean value)
```


프로젝트가 리본의 View 탭에 있는 Filter 드롭다운 목록에 필터 이름을 표시하는지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 프로젝트가 리본의 보기 탭에 있는 필터 드롭다운 목록에 필터 이름을 표시하는지 여부를 나타내는 값. |

### setShowRelatedSummaryRows(boolean value) {#setShowRelatedSummaryRows-boolean-}
```
public final void setShowRelatedSummaryRows(boolean value)
```


필터에 대해 관련 요약 행이 표시되는지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 값 | boolean | 필터에 대해 관련 요약 행이 표시되는지 여부를 나타내는 값. |

