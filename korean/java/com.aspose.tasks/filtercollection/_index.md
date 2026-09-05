---
title: "FilterCollection"
second_title: "Aspose.Tasks for Java API Reference"
description: "객체 목록을 포함합니다."
type: docs
weight: 92
url: /ko/java/com.aspose.tasks/filtercollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection
```
public class FilterCollection extends AbstractCollection<Filter>
```

[Filter](../../com.aspose.tasks/filter) 객체 목록을 포함합니다. ICollection&lt;Filter&gt; 인터페이스를 구현합니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [add(Filter item)](#add-com.aspose.tasks.Filter-) |  |
| [clear()](#clear--) | 이 컬렉션에서 모든 요소를 제거합니다 (선택적 작업). |
| [contains(Filter item)](#contains-com.aspose.tasks.Filter-) | 이 컬렉션에 지정된 항목이 포함되어 있으면 true를 반환합니다. |
| [copyTo(Filter[] array, int arrayIndex)](#copyTo-com.aspose.tasks.Filter---int-) | 지정된 인덱스부터 지정된 배열의 요소를 이 컬렉션으로 복사합니다. |
| [iterator()](#iterator--) | 이 컬렉션에 포함된 요소에 대한 반복자를 반환합니다. |
| [remove(Filter item)](#remove-com.aspose.tasks.Filter-) | 이 컬렉션에서 지정된 항목을 제거합니다. |
| [size()](#size--) | 이 컬렉션에 포함된 요소 수를 가져옵니다. |
| [toList()](#toList--) | `Filter` 객체 목록으로 필터 컬렉션을 변환합니다. |
### add(Filter item) {#add-com.aspose.tasks.Filter-}
```
public boolean add(Filter item)
```




**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| item | [Filter](../../com.aspose.tasks/filter) |  |

**Returns:**
boolean
### clear() {#clear--}
```
public void clear()
```


이 컬렉션에서 모든 요소를 제거합니다 (선택적 작업).

### contains(Filter item) {#contains-com.aspose.tasks.Filter-}
```
public final boolean contains(Filter item)
```


이 컬렉션에 지정된 항목이 포함되어 있으면 true를 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| item | [Filter](../../com.aspose.tasks/filter) | 지정된 항목. |

**Returns:**
boolean - 컬렉션에 지정된 항목이 포함되어 있으면 true.
### copyTo(Filter[] array, int arrayIndex) {#copyTo-com.aspose.tasks.Filter---int-}
```
public final void copyTo(Filter[] array, int arrayIndex)
```


지정된 인덱스부터 지정된 배열의 요소를 이 컬렉션으로 복사합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| array | [Filter\[\]](../../com.aspose.tasks/filter) | 요소를 복사할 지정된 1차원 배열 |
| arrayIndex | int | 복사가 시작되는 지정된 배열의 0부터 시작하는 인덱스. |

### iterator() {#iterator--}
```
public Iterator<Filter> iterator()
```


이 컬렉션에 포함된 요소에 대한 반복자를 반환합니다.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Filter&gt; - 컬렉션 반복자.
### remove(Filter item) {#remove-com.aspose.tasks.Filter-}
```
public final boolean remove(Filter item)
```


이 컬렉션에서 지정된 항목을 제거합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| item | [Filter](../../com.aspose.tasks/filter) | 지정된 항목. |

**Returns:**
boolean - 작업이 성공하면 true.
### size() {#size--}
```
public final int size()
```


이 컬렉션에 포함된 요소 수를 가져옵니다.

**Returns:**
int - 이 컬렉션에 포함된 요소 수.
### toList() {#toList--}
```
public List<Filter> toList()
```


`Filter` 객체 목록으로 필터 컬렉션을 변환합니다.

**Returns:**
java.util.List&lt;com.aspose.tasks.Filter&gt; - `Filter` 객체의 일반 목록.
