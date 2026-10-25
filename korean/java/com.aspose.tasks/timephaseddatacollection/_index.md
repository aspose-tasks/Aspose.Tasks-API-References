---
title: "TimephasedDataCollection"
second_title: "Aspose.Tasks for Java API Reference"
description: "객체 컬렉션을 나타냅니다."
type: docs
weight: 321
url: /ko/java/com.aspose.tasks/timephaseddatacollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public abstract class TimephasedDataCollection extends AbstractList<TimephasedData>
```

시간 구간 데이터 객체([TimephasedData](../../com.aspose.tasks/timephaseddata))의 컬렉션을 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [TimephasedDataCollection()](#TimephasedDataCollection--) | 새로운 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 클래스 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [add(TimephasedData item)](#add-com.aspose.tasks.TimephasedData-) | [TimephasedData](../../com.aspose.tasks/timephaseddata) 인스턴스를 이 컬렉션 객체에 추가합니다. |
| [addRange(Iterable&lt;TimephasedData&gt; timephasedCollection)](#addRange-java.lang.Iterable-com.aspose.tasks.TimephasedData--) | 이 컬렉션 객체에 [TimephasedData](../../com.aspose.tasks/timephaseddata) 인스턴스 컬렉션을 추가합니다. |
| [clear()](#clear--) | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection)에서 모든 항목을 제거합니다. |
| [containsItem(TimephasedData item)](#containsItem-com.aspose.tasks.TimephasedData-) | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 에 특정 값이 포함되어 있는지 확인합니다. |
| [copyToTArray(TimephasedData[] array, int arrayIndex)](#copyToTArray-com.aspose.tasks.TimephasedData---int-) | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 의 요소를 배열에 복사하며, 특정 배열 인덱스에서 시작합니다. |
| [get(int index)](#get-int-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | System.Collections.Generic.ICollection&lt;T&gt; 가 읽기 전용인지 여부를 나타내는 값을 가져옵니다. |
| [iterator()](#iterator--) | 이 컬렉션에 대한 반복자를 반환합니다. |
| [remove(TimephasedData item)](#remove-com.aspose.tasks.TimephasedData-) | 이 컬렉션 객체에서 [TimephasedData](../../com.aspose.tasks/timephaseddata) 인스턴스를 제거합니다. |
| [selectBetweenStartAndFinish(byte timephasedDataType, Date startTime, Date finishTime)](#selectBetweenStartAndFinish-byte-java.util.Date-java.util.Date-) | `startTime` 과 `finishTime` 사이의 모든 시간 구간을 선택합니다. |
| [set_Item(int index, TimephasedData value)](#set-Item-int-com.aspose.tasks.TimephasedData-) | 지정된 인덱스에 요소를 설정합니다. |
| [size()](#size--) | 이 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 객체에 포함된 객체 수를 가져옵니다. |
| [toList()](#toList--) | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 객체를 [TimephasedData](../../com.aspose.tasks/timephaseddata) 객체 목록으로 변환합니다. |
### TimephasedDataCollection() {#TimephasedDataCollection--}
```
public TimephasedDataCollection()
```


새로운 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 클래스 인스턴스를 초기화합니다.

### add(TimephasedData item) {#add-com.aspose.tasks.TimephasedData-}
```
public final boolean add(TimephasedData item)
```


[TimephasedData](../../com.aspose.tasks/timephaseddata) 인스턴스를 이 컬렉션 객체에 추가합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| item | [TimephasedData](../../com.aspose.tasks/timephaseddata) | 추가할 항목. |

**Returns:**
boolean - 항목이 추가되었으면 true; 그렇지 않으면 false.
### addRange(Iterable&lt;TimephasedData&gt; timephasedCollection) {#addRange-java.lang.Iterable-com.aspose.tasks.TimephasedData--}
```
public final void addRange(Iterable<TimephasedData> timephasedCollection)
```


이 컬렉션 객체에 [TimephasedData](../../com.aspose.tasks/timephaseddata) 인스턴스 컬렉션을 추가합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| timephasedCollection | java.lang.Iterable&lt;com.aspose.tasks.TimephasedData&gt; | 추가할 [TimephasedData](../../com.aspose.tasks/timephaseddata) 객체의 컬렉션. |

### clear() {#clear--}
```
public final void clear()
```


[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection)에서 모든 항목을 제거합니다.

### containsItem(TimephasedData item) {#containsItem-com.aspose.tasks.TimephasedData-}
```
public final boolean containsItem(TimephasedData item)
```


[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 에 특정 값이 포함되어 있는지 확인합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| item | [TimephasedData](../../com.aspose.tasks/timephaseddata) | 컬렉션에서 찾을 객체. |

**Returns:**
boolean - 컬렉션에서 `item` 이 발견되면 true; 그렇지 않으면 false.
### copyToTArray(TimephasedData[] array, int arrayIndex) {#copyToTArray-com.aspose.tasks.TimephasedData---int-}
```
public final void copyToTArray(TimephasedData[] array, int arrayIndex)
```


[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 의 요소를 배열에 복사하며, 특정 배열 인덱스에서 시작합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| array | [TimephasedData\[\]](../../com.aspose.tasks/timephaseddata) | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 로부터 복사된 요소들의 대상이 되는 1차원 배열입니다. 배열은 0부터 시작하는 인덱스를 가져야 합니다. |
| arrayIndex | int | 복사가 시작되는 `array` 의 0 기반 인덱스입니다. |

### get(int index) {#get-int-}
```
public TimephasedData get(int index)
```




**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[TimephasedData](../../com.aspose.tasks/timephaseddata) - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


System.Collections.Generic.ICollection&lt;T&gt; 가 읽기 전용인지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - System.Collections.Generic.ICollection&lt;T&gt; 가 읽기 전용이면 true; 그렇지 않으면 false.
### iterator() {#iterator--}
```
public final Iterator<TimephasedData> iterator()
```


이 컬렉션에 대한 반복자를 반환합니다.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.TimephasedData&gt; - 이 컬렉션에 대한 반복자.
### remove(TimephasedData item) {#remove-com.aspose.tasks.TimephasedData-}
```
public final boolean remove(TimephasedData item)
```


이 컬렉션 객체에서 [TimephasedData](../../com.aspose.tasks/timephaseddata) 인스턴스를 제거합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| item | [TimephasedData](../../com.aspose.tasks/timephaseddata) | 제거할 항목입니다. |

**Returns:**
boolean - `item` 이 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 에서 성공적으로 제거되었으면 true; 그렇지 않으면 false. `item` 이 해당 컬렉션에 없을 경우에도 false를 반환합니다.
### selectBetweenStartAndFinish(byte timephasedDataType, Date startTime, Date finishTime) {#selectBetweenStartAndFinish-byte-java.util.Date-java.util.Date-}
```
public final List<TimephasedData> selectBetweenStartAndFinish(byte timephasedDataType, Date startTime, Date finishTime)
```


`startTime` 과 `finishTime` 사이의 모든 시간 구간을 선택합니다. 평균 경우 O(log n) 복잡도를 가집니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| timephasedDataType | 바이트 | 선택할 시간 구간의 유형. |
| startTime | java.util.Date | 구간 시작. |
| finishTime | java.util.Date | 구간 종료. |

**Returns:**
java.util.List&lt;com.aspose.tasks.TimephasedData&gt; - [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 데이터가 Start 속성으로 정렬된 새 리스트 인스턴스를 반환합니다.
### set_Item(int index, TimephasedData value) {#set-Item-int-com.aspose.tasks.TimephasedData-}
```
public final void set_Item(int index, TimephasedData value)
```


지정된 인덱스에 요소를 설정합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| index | int | 설정할 요소의 0부터 시작하는 인덱스입니다. |
| value | [TimephasedData](../../com.aspose.tasks/timephaseddata) | 설정할 요소. |

### size() {#size--}
```
public final int size()
```


이 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 객체에 포함된 객체 수를 가져옵니다.

**Returns:**
int - 이 [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 객체에 포함된 객체 수.
### toList() {#toList--}
```
public final List<TimephasedData> toList()
```


[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) 객체를 [TimephasedData](../../com.aspose.tasks/timephaseddata) 객체 목록으로 변환합니다.

**Returns:**
java.util.List&lt;com.aspose.tasks.TimephasedData&gt; - [TimephasedData](../../com.aspose.tasks/timephaseddata) 객체들의 리스트.
