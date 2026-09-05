---
title: "ViewCollection"
second_title: "Aspose.Tasks for Java API Reference"
description: "객체 목록을 포함합니다."
type: docs
weight: 343
url: /ko/java/com.aspose.tasks/viewcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection
```
public class ViewCollection extends AbstractCollection<View>
```

[View](../../com.aspose.tasks/view) 객체의 목록을 포함합니다. `AbstractCollection` 클래스를 확장합니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [add(View item)](#add-com.aspose.tasks.View-) | 지정된 항목을 이 컬렉션에 추가합니다. |
| [clear()](#clear--) | 이 컬렉션에서 모든 항목을 제거합니다. |
| [contains(View item)](#contains-com.aspose.tasks.View-) | 지정된 항목이 이 컬렉션에 있으면 true를 반환하고, 그렇지 않으면 false를 반환합니다. |
| [copyTo(View[] array, int arrayIndex)](#copyTo-com.aspose.tasks.View---int-) | 이 컬렉션의 요소를 지정된 배열에 복사합니다. 복사는 지정된 배열 인덱스부터 시작합니다. |
| [getByName(String viewName)](#getByName-java.lang.String-) | 이름이 일치하는 View를 검색하고, 컬렉션 내에서 첫 번째 항목을 반환합니다. |
| [getByViewScreen(int screen)](#getByViewScreen-int-) | 지정된 Screen 속성을 가진 View를 검색하고, 컬렉션 내에서 첫 번째 항목을 반환합니다. |
| [getParentProject()](#getParentProject--) | View 객체의 부모를 가져옵니다. |
| [iterator()](#iterator--) | 이 컬렉션에 포함된 요소에 대한 반복자를 반환합니다. |
| [remove(View item)](#remove-com.aspose.tasks.View-) | 이 컬렉션에서 특정 객체의 첫 번째 발생을 제거합니다. |
| [size()](#size--) | 이 컬렉션에 포함된 요소 수를 가져옵니다. |
| [toList()](#toList--) | view 컬렉션을 [View](../../com.aspose.tasks/view) 객체 목록으로 변환합니다. |
### add(View item) {#add-com.aspose.tasks.View-}
```
public final boolean add(View item)
```


지정된 항목을 이 컬렉션에 추가합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | 이 컬렉션에 추가할 지정된 항목. |

**Returns:**
boolean - 작업이 성공하면 true.
### clear() {#clear--}
```
public final void clear()
```


이 컬렉션에서 모든 항목을 제거합니다.

### contains(View item) {#contains-com.aspose.tasks.View-}
```
public final boolean contains(View item)
```


지정된 항목이 이 컬렉션에 있으면 true를 반환하고, 그렇지 않으면 false를 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | 찾을 지정된 항목. |

**Returns:**
boolean - 지정된 항목이 이 컬렉션에 있으면 true, 그렇지 않으면 false.
### copyTo(View[] array, int arrayIndex) {#copyTo-com.aspose.tasks.View---int-}
```
public final void copyTo(View[] array, int arrayIndex)
```


이 컬렉션의 요소를 지정된 배열에 복사합니다. 복사는 지정된 배열 인덱스부터 시작합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| array | [View\[\]](../../com.aspose.tasks/view) | 요소를 복사할 지정된 1차원 배열 |
| arrayIndex | int | 복사가 시작되는 지정된 배열의 0부터 시작하는 인덱스. |

### getByName(String viewName) {#getByName-java.lang.String-}
```
public final View getByName(String viewName)
```


이름이 일치하는 View를 검색하고, 컬렉션 내에서 첫 번째 항목을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| viewName | java.lang.String | 검색할 View의 이름. |

**Returns:**
[View](../../com.aspose.tasks/view) - The first View in collection with the specified name, if found; otherwise, null.
### getByViewScreen(int screen) {#getByViewScreen-int-}
```
public final View getByViewScreen(int screen)
```


지정된 Screen 속성을 가진 View를 검색하고, 컬렉션 내에서 첫 번째 항목을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| screen | int | [ViewScreen](../../com.aspose.tasks/viewscreen) 열거형 값. |

**Returns:**
[View](../../com.aspose.tasks/view) - The first View in collection which Screen property matches the specified screen argument, if found; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


View 객체의 상위 항목을 가져옵니다. 읽기 전용 [Project](../../com.aspose.tasks/project).

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent of the View object.
### iterator() {#iterator--}
```
public Iterator<View> iterator()
```


이 컬렉션에 포함된 요소에 대한 반복자를 반환합니다.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.View&gt; - 컬렉션 반복자.
### remove(View item) {#remove-com.aspose.tasks.View-}
```
public final boolean remove(View item)
```


이 컬렉션에서 특정 객체의 첫 번째 발생을 제거합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| item | [View](../../com.aspose.tasks/view) | 제거할 지정된 객체. |

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
public final List<View> toList()
```


view 컬렉션을 [View](../../com.aspose.tasks/view) 객체 목록으로 변환합니다.

**Returns:**
java.util.List&lt;com.aspose.tasks.View&gt; - [View](../../com.aspose.tasks/view) 객체의 일반 목록.
