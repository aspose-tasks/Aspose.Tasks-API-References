---
title: "ReadOnlyCollectionBase"
second_title: "Aspose.Tasks for Java API Reference"
description: "읽기 전용 객체 컬렉션을 나타냅니다."
type: docs
weight: 238
url: /ko/java/com.aspose.tasks/readonlycollectionbase/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public abstract class ReadOnlyCollectionBase<T> extends AbstractList<T>
```

읽기 전용 객체 컬렉션을 나타냅니다.

T : 컬렉션 항목의 유형.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [add(T item)](#add-T-) | ICollection의 Add 메서드에 대한 스텁 구현으로, UnsupportedOperationException만 발생시킵니다. |
| [add(int index, T element)](#add-int-T-) | \{@inheritDoc\} |
| [clear()](#clear--) | \{@inheritDoc\} |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | 지정된 인덱스에 있는 요소를 반환합니다. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | 컬렉션이 읽기 전용인지 여부를 결정합니다. |
| [iterator()](#iterator--) | 이 컬렉션에 대한 열거자를 반환합니다. |
| [remove(int index)](#remove-int-) | \{@inheritDoc\} |
| [remove(Object o)](#remove-java.lang.Object-) | \{@inheritDoc\} |
| [set(int index, T value)](#set-int-T-) | 지정된 인덱스에 있는 요소를 반환합니다. |
| [size()](#size--) | 객체에 포함된 객체 수를 가져옵니다. |
| [toList()](#toList--) | 컬렉션을 객체 목록으로 변환합니다. |
### add(T item) {#add-T-}
```
public final boolean add(T item)
```


ICollection의 Add 메서드에 대한 스텁 구현으로, UnsupportedOperationException만 발생시킵니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| item | T | 추가할 항목. |

**Returns:**
boolean
### add(int index, T element) {#add-int-T-}
```
public final void add(int index, T element)
```




**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |
| 요소 | T | \{@inheritDoc\} |

### clear() {#clear--}
```
public final void clear()
```




### contains(Object o) {#contains-java.lang.Object-}
```
public final boolean contains(Object o)
```




**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### get(int index) {#get-int-}
```
public final T get(int index)
```


지정된 인덱스에 있는 요소를 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| index | int | 가져올 요소의 0부터 시작하는 인덱스입니다. |

**Returns:**
T - 지정된 인덱스의 요소.
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public final int indexOf(Object o)
```




**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
int - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


컬렉션이 읽기 전용인지 여부를 결정합니다.

**Returns:**
boolean - 컬렉션이 읽기 전용이면 true; 그렇지 않으면 false.
### iterator() {#iterator--}
```
public final Iterator<T> iterator()
```


이 컬렉션에 대한 열거자를 반환합니다.

**Returns:**
java.util.Iterator<T> - 이 컬렉션에 대한 열거자.
### remove(int index) {#remove-int-}
```
public final T remove(int index)
```




**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
T - {@inheritDoc}
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```




**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### set(int index, T value) {#set-int-T-}
```
public final T set(int index, T value)
```


지정된 인덱스에 있는 요소를 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| index | int | 가져올 요소의 0부터 시작하는 인덱스입니다. |
| 값 | T |  |

**Returns:**
T - 지정된 인덱스의 요소.
### size() {#size--}
```
public final int size()
```


객체에 포함된 객체 수를 가져옵니다.

**Returns:**
int - 객체에 포함된 객체 수.
### toList() {#toList--}
```
public final List<T> toList()
```


컬렉션을 객체 목록으로 변환합니다.

**Returns:**
java.util.List<T> - 객체의 일반 리스트.
