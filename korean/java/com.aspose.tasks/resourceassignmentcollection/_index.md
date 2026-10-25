---
title: "ResourceAssignmentCollection"
second_title: "Aspose.Tasks for Java API Reference"
description: "객체 컬렉션을 나타냅니다."
type: docs
weight: 250
url: /ko/java/com.aspose.tasks/resourceassignmentcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class ResourceAssignmentCollection extends AbstractList<ResourceAssignment>
```

다음 [ResourceAssignment](../../com.aspose.tasks/resourceassignment) 객체들의 컬렉션을 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [add(ResourceAssignment item)](#add-com.aspose.tasks.ResourceAssignment-) | ICollection의 Add 메서드에 대한 스텁 구현으로, UnsupportedOperationException만 발생시킵니다. |
| [add(Task task, Resource resource)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-) | 새 할당을 ResourceAssignmentCollection에 추가합니다. |
| [add(Task task, Resource resource, double units)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-double-) | 새 할당을 ResourceAssignmentCollection에 추가합니다. |
| [add(Task task, Resource resource, BigDecimal cost)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-java.math.BigDecimal-) | 새 할당을 ResourceAssignmentCollection에 추가합니다. |
| [clear()](#clear--) | 컬렉션에서 모든 항목을 제거합니다. |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getByUid(int uid)](#getByUid-int-) | 지정된 uid를 가진 할당을 반환합니다. |
| [getParentProject()](#getParentProject--) | ResourceAssignmentCollection 객체의 상위 프로젝트를 가져옵니다. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | 이 컬렉션이 읽기 전용인지 여부를 나타내는 값을 가져옵니다. |
| [iterator()](#iterator--) | 이 컬렉션에 대한 열거자를 반환합니다. |
| [remove(int index)](#remove-int-) | \{@inheritDoc\} |
| [remove(Object o)](#remove-java.lang.Object-) | 컬렉션에서 지정된 할당을 제거합니다. 읽기 전용이 아닌 경우에만 제거되며, 그렇지 않으면 UnsupportedOperationException을 발생시킵니다. |
| [size()](#size--) | ResourceAssignmentCollection에 포함된 객체 수를 가져옵니다. |
| [toList()](#toList--) | ResourceAssignmentCollection 객체를 [ResourceAssignment](../../com.aspose.tasks/resourceassignment) 객체 목록으로 변환합니다. |
### add(ResourceAssignment item) {#add-com.aspose.tasks.ResourceAssignment-}
```
public final boolean add(ResourceAssignment item)
```


ICollection의 Add 메서드에 대한 스텁 구현으로, UnsupportedOperationException만 발생시킵니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| item | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | 제거할 항목입니다. |

**Returns:**
boolean - \{@inheritDoc\}
### add(Task task, Resource resource) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-}
```
public final ResourceAssignment add(Task task, Resource resource)
```


새 할당을 ResourceAssignmentCollection에 추가합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | 할당될 작업. |
| resource | [Resource](../../com.aspose.tasks/resource) | 할당될 리소스. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### add(Task task, Resource resource, double units) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-double-}
```
public final ResourceAssignment add(Task task, Resource resource, double units)
```


새 할당을 ResourceAssignmentCollection에 추가합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | 할당될 작업. |
| resource | [Resource](../../com.aspose.tasks/resource) | 할당될 리소스. |
| 단위 | double | 새 할당에 대한 단위 수. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### add(Task task, Resource resource, BigDecimal cost) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-java.math.BigDecimal-}
```
public final ResourceAssignment add(Task task, Resource resource, BigDecimal cost)
```


새 할당을 ResourceAssignmentCollection에 추가합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | 할당될 작업. |
| resource | [Resource](../../com.aspose.tasks/resource) | 할당될 비용 리소스. |
| 비용 | java.math.BigDecimal | 새 할당에 대한 비용. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### clear() {#clear--}
```
public void clear()
```


컬렉션에서 모든 항목을 제거합니다.

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
public ResourceAssignment get(int index)
```


(@inheritDoc\}

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - \{@inheritDoc\}
### getByUid(int uid) {#getByUid-int-}
```
public final ResourceAssignment getByUid(int uid)
```


지정된 uid를 가진 할당을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | uid | int | 지정된 uid. |

--------------------

O(1) 복잡도. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - ResourceAssignment with the specified uid if present; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


ResourceAssignmentCollection 객체의 상위 프로젝트를 가져옵니다.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the ResourceAssignmentCollection object.
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


이 컬렉션이 읽기 전용인지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean - 이 컬렉션이 읽기 전용인지 여부를 나타내는 값.
### iterator() {#iterator--}
```
public final Iterator<ResourceAssignment> iterator()
```


이 컬렉션에 대한 열거자를 반환합니다.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.ResourceAssignment&gt; - 이 컬렉션에 대한 열거자.
### remove(int index) {#remove-int-}
```
public ResourceAssignment remove(int index)
```




**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - \{@inheritDoc\}
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```


컬렉션에서 지정된 할당을 제거합니다. 읽기 전용이 아닌 경우에만 제거되며, 그렇지 않으면 UnsupportedOperationException을 발생시킵니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| o | java.lang.Object | 제거할 할당. |

**Returns:**
boolean - 지정된 항목이 제거되면 true, 그렇지 않으면 false.
### size() {#size--}
```
public final int size()
```


ResourceAssignmentCollection에 포함된 객체 수를 가져옵니다.

**Returns:**
int - ResourceAssignmentCollection에 포함된 객체 수.
### toList() {#toList--}
```
public final List<ResourceAssignment> toList()
```


ResourceAssignmentCollection 객체를 [ResourceAssignment](../../com.aspose.tasks/resourceassignment) 객체 목록으로 변환합니다.

**Returns:**
java.util.List&lt;com.aspose.tasks.ResourceAssignment&gt; - [ResourceAssignment](../../com.aspose.tasks/resourceassignment) 객체들의 리스트.
