---
title: "TableCollection"
second_title: "Aspose.Tasks for Java API Reference"
description: "객체 목록을 포함합니다."
type: docs
weight: 285
url: /ko/java/com.aspose.tasks/tablecollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection
```
public class TableCollection extends AbstractCollection<Table>
```

객체 목록에 [Table](../../com.aspose.tasks/table) 객체를 포함합니다. ICollection&lt;Table&gt; 인터페이스를 구현합니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [add(Table item)](#add-com.aspose.tasks.Table-) | 지정된 항목을 이 컬렉션에 추가합니다. |
| [clear()](#clear--) | 이 컬렉션에서 모든 항목을 제거합니다. |
| [contains(Table item)](#contains-com.aspose.tasks.Table-) | 지정된 항목이 이 컬렉션에 있으면 true를 반환하고, 그렇지 않으면 false를 반환합니다. |
| [copyTo(Table[] array, int arrayIndex)](#copyTo-com.aspose.tasks.Table---int-) | 이 컬렉션의 요소를 지정된 배열에 복사합니다. 복사는 지정된 배열 인덱스부터 시작합니다. |
| [iterator()](#iterator--) | 이 컬렉션에 대한 열거자를 반환합니다. |
| [remove(Table item)](#remove-com.aspose.tasks.Table-) | 이 컬렉션에서 특정 객체의 첫 번째 발생을 제거합니다. |
| [size()](#size--) | 이 컬렉션에 포함된 요소 수를 가져옵니다. |
| [toList()](#toList--) | 테이블 컬렉션을 [Table](../../com.aspose.tasks/table) 객체 목록으로 변환합니다. |
### add(Table item) {#add-com.aspose.tasks.Table-}
```
public final boolean add(Table item)
```


지정된 항목을 이 컬렉션에 추가합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| item | [Table](../../com.aspose.tasks/table) | 이 컬렉션에 추가할 지정된 항목. |

**Returns:**
boolean - 추가 작업이 성공하고 항목이 컬렉션에 추가된 경우 true.
### clear() {#clear--}
```
public final void clear()
```


이 컬렉션에서 모든 항목을 제거합니다.

### contains(Table item) {#contains-com.aspose.tasks.Table-}
```
public final boolean contains(Table item)
```


지정된 항목이 이 컬렉션에 있으면 true를 반환하고, 그렇지 않으면 false를 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| item | [Table](../../com.aspose.tasks/table) | 찾을 지정된 항목. |

**Returns:**
boolean - 지정된 항목이 이 컬렉션에 있으면 true, 그렇지 않으면 false.
### copyTo(Table[] array, int arrayIndex) {#copyTo-com.aspose.tasks.Table---int-}
```
public final void copyTo(Table[] array, int arrayIndex)
```


이 컬렉션의 요소를 지정된 배열에 복사합니다. 복사는 지정된 배열 인덱스부터 시작합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| array | [Table\[\]](../../com.aspose.tasks/table) | 요소를 복사할 지정된 1차원 배열 |
| arrayIndex | int | 복사가 시작되는 지정된 배열의 0부터 시작하는 인덱스. |

### iterator() {#iterator--}
```
public final Iterator<Table> iterator()
```


이 컬렉션에 대한 열거자를 반환합니다.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Table&gt; - 이 컬렉션에 대한 열거자.
### remove(Table item) {#remove-com.aspose.tasks.Table-}
```
public final boolean remove(Table item)
```


이 컬렉션에서 특정 객체의 첫 번째 발생을 제거합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| item | [Table](../../com.aspose.tasks/table) | 제거할 지정된 객체. |

**Returns:**
boolean - 지정된 객체가 이 컬렉션에서 성공적으로 제거되면 true; 그렇지 않으면 false.
### size() {#size--}
```
public final int size()
```


이 컬렉션에 포함된 요소 수를 가져옵니다.

**Returns:**
int - 이 컬렉션에 포함된 요소 수.
### toList() {#toList--}
```
public final List<Table> toList()
```


테이블 컬렉션을 [Table](../../com.aspose.tasks/table) 객체 목록으로 변환합니다.

**Returns:**
java.util.List&lt;com.aspose.tasks.Table&gt; - [Table](../../com.aspose.tasks/table) 객체의 일반 리스트.
