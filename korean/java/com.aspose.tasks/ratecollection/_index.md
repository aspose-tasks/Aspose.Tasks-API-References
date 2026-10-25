---
title: "RateCollection"
second_title: "Aspose.Tasks for Java API Reference"
description: "객체를 포함하는 컬렉션을 나타냅니다."
type: docs
weight: 234
url: /ko/java/com.aspose.tasks/ratecollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractMap

**All Implemented Interfaces:**
java.lang.Iterable
```
public class RateCollection extends AbstractMap<Integer,RateByDateCollection> implements Iterable<Map.Entry<Integer,RateByDateCollection>>
```

컬렉션은 [Rate](../../com.aspose.tasks/rate) 객체를 포함합니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [add(Date ratesFrom)](#add-java.util.Date-) | 새로운 [Rate](../../com.aspose.tasks/rate) 인스턴스를 이 컬렉션에 추가합니다. |
| [add(Date ratesFrom, int type)](#add-java.util.Date-int-) | 새로운 [Rate](../../com.aspose.tasks/rate) 인스턴스를 이 컬렉션에 추가합니다. |
| [clear()](#clear--) | \{@inheritDoc\} |
| [entrySet()](#entrySet--) | (@inheritDoc\} |
| [get(Object key)](#get-java.lang.Object-) | (@inheritDoc\} |
| [getByRateType(int key)](#getByRateType-int-) | 지정된 인덱스에 있는 요소를 반환합니다. |
| [getParentResource()](#getParentResource--) | 이 컬렉션에 대한 상위 [Resource](../../com.aspose.tasks/resource) 객체를 가져옵니다. |
| [isReadOnly()](#isReadOnly--) | 이 컬렉션이 읽기 전용인지 여부를 나타내는 값을 가져옵니다. |
| [iterator()](#iterator--) | 이 컬렉션에 대한 열거자를 반환합니다. |
| [put(Integer key, RateByDateCollection value)](#put-java.lang.Integer-com.aspose.tasks.RateByDateCollection-) | (@inheritDoc\} |
| [remove(Rate item)](#remove-com.aspose.tasks.Rate-) | 이 컬렉션에서 Rate 인스턴스를 제거합니다. |
| [setByRateType(int key, RateByDateCollection value)](#setByRateType-int-com.aspose.tasks.RateByDateCollection-) | 지정된 인덱스에 요소를 설정합니다. |
| [size()](#size--) | RateCollection에 포함된 요소의 수를 가져옵니다. |
| [toList()](#toList--) | [RateCollection](../../com.aspose.tasks/ratecollection) 객체를 [Rate](../../com.aspose.tasks/rate) 객체 목록으로 변환합니다. |
| [toList(int type)](#toList-int-) | [RateCollection](../../com.aspose.tasks/ratecollection) 객체를 지정된 [RateType](../../com.aspose.tasks/ratetype) 유형으로 필터링된 [Rate](../../com.aspose.tasks/rate) 객체 목록으로 변환합니다. |
### add(Date ratesFrom) {#add-java.util.Date-}
```
public final Rate add(Date ratesFrom)
```


새로운 [Rate](../../com.aspose.tasks/rate) 인스턴스를 이 컬렉션에 추가합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| ratesFrom | java.util.Date | 새 요금이 적용되는 날짜입니다. |

**Returns:**
[Rate](../../com.aspose.tasks/rate) - Added [Rate](../../com.aspose.tasks/rate) instance.
### add(Date ratesFrom, int type) {#add-java.util.Date-int-}
```
public final Rate add(Date ratesFrom, int type)
```


새로운 [Rate](../../com.aspose.tasks/rate) 인스턴스를 이 컬렉션에 추가합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| ratesFrom | java.util.Date | 새 요금이 적용되는 날짜입니다. |
| type | int | 추가할 요금표입니다. |

**Returns:**
[Rate](../../com.aspose.tasks/rate) - Added [Rate](../../com.aspose.tasks/rate) instance.
### clear() {#clear--}
```
public final void clear()
```




### entrySet() {#entrySet--}
```
public Set<Map.Entry<Integer,RateByDateCollection>> entrySet()
```


(@inheritDoc\}

**Returns:**
java.util.Set&lt;java.util.Map.Entry&lt;java.lang.Integer,com.aspose.tasks.RateByDateCollection&gt;&gt; - \{@inheritDoc\}
### get(Object key) {#get-java.lang.Object-}
```
public final RateByDateCollection get(Object key)
```


(@inheritDoc\}

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| key | java.lang.Object | \{@inheritDoc\} |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - \{@inheritDoc\}
### getByRateType(int key) {#getByRateType-int-}
```
public final RateByDateCollection getByRateType(int key)
```


지정된 인덱스에 있는 요소를 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| key | int | 가져올 요소의 0부터 시작하는 인덱스입니다. |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - the element at the specified index.
### getParentResource() {#getParentResource--}
```
public final Resource getParentResource()
```


이 컬렉션에 대한 상위 [Resource](../../com.aspose.tasks/resource) 객체를 가져옵니다.

**Returns:**
[Resource](../../com.aspose.tasks/resource) - the parent [Resource](../../com.aspose.tasks/resource) object for this collection.
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


이 컬렉션이 읽기 전용인지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 이 컬렉션이 읽기 전용인지 여부를 나타내는 값.
### iterator() {#iterator--}
```
public final Iterator iterator()
```


이 컬렉션에 대한 열거자를 반환합니다.

**Returns:**
java.util.Iterator - 이 컬렉션에 대한 열거자.
### put(Integer key, RateByDateCollection value) {#put-java.lang.Integer-com.aspose.tasks.RateByDateCollection-}
```
public final RateByDateCollection put(Integer key, RateByDateCollection value)
```


(@inheritDoc\}

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| key | java.lang.Integer | \{@inheritDoc\} |
| value | [RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) | \{@inheritDoc\} |

**Returns:**
[RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) - \{@inheritDoc\}
### remove(Rate item) {#remove-com.aspose.tasks.Rate-}
```
public final boolean remove(Rate item)
```


이 컬렉션에서 Rate 인스턴스를 제거합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| item | [Rate](../../com.aspose.tasks/rate) | 제거할 항목입니다. |

**Returns:**
boolean - 지정된 Rate가 성공적으로 제거된 경우 true; 그렇지 않으면 false.
### setByRateType(int key, RateByDateCollection value) {#setByRateType-int-com.aspose.tasks.RateByDateCollection-}
```
public final void setByRateType(int key, RateByDateCollection value)
```


지정된 인덱스에 요소를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| key | int | 설정할 요소의 0부터 시작하는 인덱스입니다. |
| value | [RateByDateCollection](../../com.aspose.tasks/ratebydatecollection) | 지정된 인덱스에 설정할 요소입니다. |

### size() {#size--}
```
public final int size()
```


RateCollection에 포함된 요소의 수를 가져옵니다.

**Returns:**
int - RateCollection에 포함된 요소 수입니다.
### toList() {#toList--}
```
public final List<Rate> toList()
```


[RateCollection](../../com.aspose.tasks/ratecollection) 객체를 [Rate](../../com.aspose.tasks/rate) 객체 목록으로 변환합니다.

**Returns:**
java.util.List&lt;com.aspose.tasks.Rate&gt; - [Rate](../../com.aspose.tasks/rate) 객체 목록입니다.
### toList(int type) {#toList-int-}
```
public final List<Rate> toList(int type)
```


[RateCollection](../../com.aspose.tasks/ratecollection) 객체를 지정된 [RateType](../../com.aspose.tasks/ratetype) 유형으로 필터링된 [Rate](../../com.aspose.tasks/rate) 객체 목록으로 변환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| type | int | 필터링할 유형입니다. |

**Returns:**
java.util.List&lt;com.aspose.tasks.Rate&gt; - [Rate](../../com.aspose.tasks/rate) 객체 목록입니다.
