---
title: "WeekDayCollection"
second_title: "Aspose.Tasks for Java API Reference"
description: "객체 컬렉션을 나타냅니다."
type: docs
weight: 353
url: /ko/java/com.aspose.tasks/weekdaycollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList

**All Implemented Interfaces:**
java.lang.Iterable
```
public class WeekDayCollection extends AbstractList<WeekDay> implements Iterable<WeekDay>
```

다음 [WeekDay](../../com.aspose.tasks/weekday) 객체들의 컬렉션을 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [add(WeekDay item)](#add-com.aspose.tasks.WeekDay-) | 이 객체에 [WeekDay](../../com.aspose.tasks/weekday) 인스턴스를 추가합니다. |
| [add(int index, WeekDay item)](#add-int-com.aspose.tasks.WeekDay-) | 지정된 인덱스에 [WeekDay](../../com.aspose.tasks/weekday)을 삽입합니다. |
| [clear()](#clear--) | WeekDayCollection 객체를 초기화합니다. |
| [contains(WeekDay item)](#contains-com.aspose.tasks.WeekDay-) | 컬렉션에 지정된 [WeekDay](../../com.aspose.tasks/weekday)이 포함되어 있는지 확인합니다. |
| [copyTo(WeekDay[] array, int arrayIndex)](#copyTo-com.aspose.tasks.WeekDay---int-) | 컬렉션 내용을 지정된 인덱스의 배열에 복사합니다. |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [indexOf(WeekDay item)](#indexOf-com.aspose.tasks.WeekDay-) | 지정된 [WeekDay](../../com.aspose.tasks/weekday)의 인덱스를 반환합니다. |
| [isReadOnly()](#isReadOnly--) | \{@inheritDoc\} |
| [iterator()](#iterator--) | 이 컬렉션에 대한 열거자를 반환합니다. |
| [remove(int index)](#remove-int-) | \{@inheritDoc\} |
| [remove(Object obj)](#remove-java.lang.Object-) | 지정된 [WeekDay](../../com.aspose.tasks/weekday)이 있으면 제거합니다. |
| [size()](#size--) | 이 [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) 객체에 포함된 객체 수를 가져옵니다. |
| [toList()](#toList--) | WeekDayCollection 객체를 [WeekDay](../../com.aspose.tasks/weekday) 객체 목록으로 변환합니다. |
### add(WeekDay item) {#add-com.aspose.tasks.WeekDay-}
```
public final boolean add(WeekDay item)
```


이 객체에 [WeekDay](../../com.aspose.tasks/weekday) 인스턴스를 추가합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| item | [WeekDay](../../com.aspose.tasks/weekday) | 추가할 항목. |

**Returns:**
boolean - \{@inheritDoc\}
### add(int index, WeekDay item) {#add-int-com.aspose.tasks.WeekDay-}
```
public final void add(int index, WeekDay item)
```


지정된 인덱스에 [WeekDay](../../com.aspose.tasks/weekday)을 삽입합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| index | int | 삽입할 인덱스. |
| item | [WeekDay](../../com.aspose.tasks/weekday) | 삽입할 [WeekDay](../../com.aspose.tasks/weekday). |

### clear() {#clear--}
```
public final void clear()
```


WeekDayCollection 객체를 초기화합니다.

### contains(WeekDay item) {#contains-com.aspose.tasks.WeekDay-}
```
public final boolean contains(WeekDay item)
```


컬렉션에 지정된 [WeekDay](../../com.aspose.tasks/weekday)이 포함되어 있는지 확인합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| item | [WeekDay](../../com.aspose.tasks/weekday) | 비교할 항목. |

**Returns:**
boolean - 컬렉션에 지정된 항목이 포함되어 있으면 true, 그렇지 않으면 false.
### copyTo(WeekDay[] array, int arrayIndex) {#copyTo-com.aspose.tasks.WeekDay---int-}
```
public final void copyTo(WeekDay[] array, int arrayIndex)
```


컬렉션 내용을 지정된 인덱스의 배열에 복사합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| array | [WeekDay\[\]](../../com.aspose.tasks/weekday) | 복사 대상이 되는 [WeekDay](../../com.aspose.tasks/weekday) 배열 |
| arrayIndex | int | 복사 작업의 시작 인덱스. |

### get(int index) {#get-int-}
```
public final WeekDay get(int index)
```


(@inheritDoc\}

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[WeekDay](../../com.aspose.tasks/weekday) - \{@inheritDoc\}
### indexOf(WeekDay item) {#indexOf-com.aspose.tasks.WeekDay-}
```
public final int indexOf(WeekDay item)
```


지정된 [WeekDay](../../com.aspose.tasks/weekday)의 인덱스를 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| item | [WeekDay](../../com.aspose.tasks/weekday) | 비교할 항목. |

**Returns:**
int - 지정된 [WeekDay](../../com.aspose.tasks/weekday)의 0 기반 인덱스(존재하면), 없으면 -1.
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```




**Returns:**
boolean - \{@inheritDoc\}
### iterator() {#iterator--}
```
public final Iterator<WeekDay> iterator()
```


이 컬렉션에 대한 열거자를 반환합니다.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.WeekDay&gt; - 이 컬렉션의 열거자.
### remove(int index) {#remove-int-}
```
public final WeekDay remove(int index)
```




**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[WeekDay](../../com.aspose.tasks/weekday) - \{@inheritDoc\}
### remove(Object obj) {#remove-java.lang.Object-}
```
public final boolean remove(Object obj)
```


지정된 [WeekDay](../../com.aspose.tasks/weekday)이 있으면 제거합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
boolean - [WeekDay](../../com.aspose.tasks/weekday)이 제거되면 True, 해당 항목을 찾지 못하면 false.
### size() {#size--}
```
public final int size()
```


이 [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) 객체에 포함된 객체 수를 가져옵니다.

**Returns:**
int - 이 [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) 객체에 포함된 객체 수.
### toList() {#toList--}
```
public final List<WeekDay> toList()
```


WeekDayCollection 객체를 [WeekDay](../../com.aspose.tasks/weekday) 객체 목록으로 변환합니다.

**Returns:**
java.util.List&lt;com.aspose.tasks.WeekDay&gt; - [WeekDay](../../com.aspose.tasks/weekday) 객체 목록.
