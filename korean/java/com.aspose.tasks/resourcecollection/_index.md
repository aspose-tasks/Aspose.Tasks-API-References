---
title: "ResourceCollection"
second_title: "Aspose.Tasks for Java API Reference"
description: "객체 컬렉션을 나타냅니다."
type: docs
weight: 251
url: /ko/java/com.aspose.tasks/resourcecollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class ResourceCollection extends AbstractList<Resource>
```

다음의 [Resource](../../com.aspose.tasks/resource) 객체 컬렉션을 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [add()](#add--) | 프로젝트 리소스 컬렉션의 마지막 위치에 새 리소스를 추가합니다. |
| [add(Resource e)](#add-com.aspose.tasks.Resource-) | \{@inheritDoc\} |
| [add(String resourceName)](#add-java.lang.String-) | 프로젝트 리소스 컬렉션의 마지막 위치에 새 리소스를 추가합니다. |
| [add(String resourceName, int beforeResourceId)](#add-java.lang.String-int-) | 프로젝트 리소스 컬렉션의 지정된 위치에 새 리소스를 추가합니다. |
| [clear()](#clear--) | 직접 삭제는 지원되지 않으며, 이 메서드는 UnsupportedOperationException을 발생시킵니다. |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getById(int id)](#getById-int-) | 지정된 id를 가진 리소스를 반환합니다. |
| [getByUid(int uid)](#getByUid-int-) | 지정된 Uid를 가진 리소스를 반환합니다. |
| [getParentProject()](#getParentProject--) | ResourceCollection 객체의 상위 프로젝트를 가져옵니다. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | \{@inheritDoc\} |
| [iterator()](#iterator--) | 이 컬렉션에 대한 열거자를 반환합니다. |
| [remove(Object o)](#remove-java.lang.Object-) | 이는 Collection의 remove 메서드에 대한 스텁 구현으로, UnsupportedOperationException만 발생시킵니다. |
| [size()](#size--) | ResourceCollection에 포함된 요소 수를 가져옵니다. |
| [sort(Comparator&lt;? super Resource&gt; comparer)](#sort-java.util.Comparator---super-com.aspose.tasks.Resource--) | \{@inheritDoc\} |
| [toList()](#toList--) | ResourceCollection 객체를 [Resource](../../com.aspose.tasks/resource) 객체 목록으로 변환합니다. |
### add() {#add--}
```
public final Resource add()
```


프로젝트 리소스 컬렉션의 마지막 위치에 새 리소스를 추가합니다.

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### add(Resource e) {#add-com.aspose.tasks.Resource-}
```
public final boolean add(Resource e)
```




**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| e | [Resource](../../com.aspose.tasks/resource) | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### add(String resourceName) {#add-java.lang.String-}
```
public final Resource add(String resourceName)
```


프로젝트 리소스 컬렉션의 마지막 위치에 새 리소스를 추가합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| resourceName | java.lang.String | 리소스의 이름. |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### add(String resourceName, int beforeResourceId) {#add-java.lang.String-int-}
```
public final Resource add(String resourceName, int beforeResourceId)
```


프로젝트 리소스 컬렉션의 지정된 위치에 새 리소스를 추가합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| resourceName | java.lang.String | 리소스의 이름. |
| beforeResourceId | int | 프로젝트 리소스 컬렉션에서 이전 리소스의 위치. |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### clear() {#clear--}
```
public final void clear()
```


직접 삭제는 지원되지 않으며, 이 메서드는 UnsupportedOperationException을 발생시킵니다.

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
public Resource get(int index)
```


(@inheritDoc\}

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - \{@inheritDoc\}
### getById(int id) {#getById-int-}
```
public final Resource getById(int id)
```


지정된 id를 가진 리소스를 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | id | int | 지정된 ID. |

--------------------

O(1) 복잡도. |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Resource with the specified id if present; otherwise, null.
### getByUid(int uid) {#getByUid-int-}
```
public final Resource getByUid(int uid)
```


지정된 Uid를 가진 리소스를 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | uid | int | 지정된 uid. |

--------------------

O(1) 복잡도. |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Resource with the specified uid if present; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


ResourceCollection 객체의 상위 프로젝트를 가져옵니다.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the ResourceCollection object.
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




**Returns:**
boolean - \{@inheritDoc\}
### iterator() {#iterator--}
```
public final Iterator<Resource> iterator()
```


이 컬렉션에 대한 열거자를 반환합니다.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Resource&gt; - 이 컬렉션에 대한 열거자.
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```


이는 Collection의 remove 메서드에 대한 스텁 구현으로, UnsupportedOperationException만 발생시킵니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| o | java.lang.Object | 제거할 항목. |

**Returns:**
boolean - 항목이 제거되었으면 `true`; 그렇지 않으면 `false`.
### size() {#size--}
```
public final int size()
```


ResourceCollection에 포함된 요소 수를 가져옵니다.

--------------------

읽기 전용 `int`.

**Returns:**
int - ResourceCollection에 포함된 요소 수.
### sort(Comparator&lt;? super Resource&gt; comparer) {#sort-java.util.Comparator---super-com.aspose.tasks.Resource--}
```
public final void sort(Comparator<? super Resource> comparer)
```




**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 비교자 | java.util.Comparator&lt;? super com.aspose.tasks.Resource&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<Resource> toList()
```


ResourceCollection 객체를 [Resource](../../com.aspose.tasks/resource) 객체 목록으로 변환합니다.

**Returns:**
java.util.List&lt;com.aspose.tasks.Resource&gt; - [Resource](../../com.aspose.tasks/resource) 객체의 목록.
