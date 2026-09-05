---
title: "TaskCollection"
second_title: "Aspose.Tasks for Java API Reference"
description: "객체 컬렉션을 나타냅니다."
type: docs
weight: 293
url: /ko/java/com.aspose.tasks/taskcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class TaskCollection extends AbstractList<Task>
```

[Task](../../com.aspose.tasks/task) 객체의 컬렉션을 나타냅니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [add()](#add--) | 마지막 작업과 동일한 개요 수준에서 프로젝트 작업 컬렉션에 새 작업을 추가합니다. |
| [add(RecurringTaskParameters parameters)](#add-com.aspose.tasks.RecurringTaskParameters-) | 지정된 ID를 가진 작업 앞에 동일한 개요 수준에서 새 작업을 삽입합니다. |
| [add(Task item)](#add-com.aspose.tasks.Task-) | 지정된 작업을 [TaskCollection](../../com.aspose.tasks/taskcollection) 클래스의 인스턴스에 추가합니다. |
| [add(String taskName)](#add-java.lang.String-) | 하위 작업 컬렉션에 새 작업을 추가합니다. |
| [add(String taskName, int beforeTaskId)](#add-java.lang.String-int-) | 하위 작업 컬렉션에 새 반복 작업을 추가합니다. |
| [clear()](#clear--) | \{@inheritDoc\} |
| [contains(Task item)](#contains-com.aspose.tasks.Task-) | 컬렉션에 지정된 항목이 포함되어 있는지 확인합니다. |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getById(int id)](#getById-int-) | 이 컬렉션의 상위 작업인 조상 작업을 가진 지정된 Id의 작업을 반환합니다. |
| [getByUid(int uid)](#getByUid-int-) | 이 컬렉션의 상위 작업인 조상 작업을 가진 지정된 Uid의 작업을 반환합니다. |
| [getParentProject()](#getParentProject--) | TaskCollection 객체의 상위 프로젝트를 가져옵니다. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | 이 컬렉션이 읽기 전용인지 여부를 나타내는 값을 가져옵니다. |
| [iterator()](#iterator--) | 이 컬렉션에 대한 열거자를 반환합니다. |
| [remove(Object item)](#remove-java.lang.Object-) | ICollection의 Remove 메서드에 대한 스텁 구현으로, UnsupportedOperationException만 발생시�니다. |
| [size()](#size--) | TaskCollection에 포함된 객체 수를 가져옵니다. |
| [sort(Comparator&lt;? super Task&gt; c)](#sort-java.util.Comparator---super-com.aspose.tasks.Task--) | \{@inheritDoc\} |
| [toList()](#toList--) | TaskCollection 객체를 [Task](../../com.aspose.tasks/task) 객체 목록으로 변환합니다. |
### add() {#add--}
```
public final Task add()
```


마지막 작업과 동일한 개요 수준에서 프로젝트 작업 컬렉션에 새 작업을 추가합니다.

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(RecurringTaskParameters parameters) {#add-com.aspose.tasks.RecurringTaskParameters-}
```
public final Task add(RecurringTaskParameters parameters)
```


지정된 ID를 가진 작업 앞에 동일한 개요 수준에서 새 작업을 삽입합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| parameters | [RecurringTaskParameters](../../com.aspose.tasks/recurringtaskparameters) | 반복 작업 생성을 위한 지정된 매개변수. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(Task item) {#add-com.aspose.tasks.Task-}
```
public final boolean add(Task item)
```


지정된 작업을 [TaskCollection](../../com.aspose.tasks/taskcollection) 클래스의 인스턴스에 추가합니다. ParentProject.CalculationMode가 None인 경우, 사용자는 이 메서드 사용 후 Project.Recalculate()를 호출해야 합니다(이 메서드는 모든 프로젝트 작업의 시작/종료 날짜를 재조정하고(조기/지연 날짜를 설정) 여유시간, 작업 및 비용 필드, ID 및 개요 수준과 같은 종속 필드를 계산합니다). ParentProject.CalculationMode가 Manual인 경우, 메서드는 작업 ID, 개요 수준 및 개요 번호만 자동으로 계산합니다. ParentProject.CalculationMode가 Automatic인 경우, 메서드는 모든 프로젝트 작업을 자동으로 재조정합니다(시작/종료 날짜를 재조정하고, 조기/지연 날짜를 설정하며, 여유시간, 작업 및 비용 필드를 계산하고, ID와 개요 수준을 재계산합니다)).

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| item | [Task](../../com.aspose.tasks/task) | 이 작업 컬렉션에 추가되어야 하는 지정된 작업. |

**Returns:**
boolean - 작업이 성공했을 경우 true.
### add(String taskName) {#add-java.lang.String-}
```
public final Task add(String taskName)
```


하위 작업 컬렉션에 새 작업을 추가합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| taskName | java.lang.String | 지정된 작업 이름. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(String taskName, int beforeTaskId) {#add-java.lang.String-int-}
```
public final Task add(String taskName, int beforeTaskId)
```


하위 작업 컬렉션에 새 반복 작업을 추가합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| taskName | java.lang.String | 지정된 작업 이름. |
| beforeTaskId | int | 새 작업이 삽입될 작업 앞에 있는 지정된 ID. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns a task which was inserted before a task with the specified id.
### clear() {#clear--}
```
public final void clear()
```




### contains(Task item) {#contains-com.aspose.tasks.Task-}
```
public final boolean contains(Task item)
```


컬렉션에 지정된 항목이 포함되어 있는지 확인합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| item | [Task](../../com.aspose.tasks/task) | 확인할 항목. |

**Returns:**
boolean - 컬렉션에 항목이 포함되어 있으면 true, 그렇지 않으면 false.
### get(int index) {#get-int-}
```
public Task get(int index)
```


(@inheritDoc\}

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[Task](../../com.aspose.tasks/task) - \{@inheritDoc\}
### getById(int id) {#getById-int-}
```
public final Task getById(int id)
```


이 컬렉션의 상위 작업인 조상 작업을 가진 지정된 Id의 작업을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| id | int | TaskEntity Id |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the instance of [Task](../../com.aspose.tasks/task) class with the specified id whose ancestor is parent task of this collection.
### getByUid(int uid) {#getByUid-int-}
```
public final Task getByUid(int uid)
```


이 컬렉션의 상위 작업인 조상 작업을 가진 지정된 Uid의 작업을 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| uid | int | TaskEntity Uid. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the instance of [Task](../../com.aspose.tasks/task) class with the specified uid whose ancestor is parent task of this collection.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


TaskCollection 객체의 상위 프로젝트를 가져옵니다.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the TaskCollection object.
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
public final Iterator<Task> iterator()
```


이 컬렉션에 대한 열거자를 반환합니다.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Task&gt; - 이 컬렉션에 대한 열거자.
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


ICollection의 Remove 메서드에 대한 스텁 구현으로, UnsupportedOperationException만 발생시�니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| item | java.lang.Object | 제거할 항목입니다. |

**Returns:**
boolean - 항목이 제거되었으면 `true`; 그렇지 않으면 `false`.
### size() {#size--}
```
public final int size()
```


TaskCollection에 포함된 객체 수를 가져옵니다.

**Returns:**
int - TaskCollection에 포함된 객체 수.
### sort(Comparator&lt;? super Task&gt; c) {#sort-java.util.Comparator---super-com.aspose.tasks.Task--}
```
public final void sort(Comparator<? super Task> c)
```




**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| c | java.util.Comparator&lt;? super com.aspose.tasks.Task&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<Task> toList()
```


TaskCollection 객체를 [Task](../../com.aspose.tasks/task) 객체 목록으로 변환합니다.

**Returns:**
java.util.List&lt;com.aspose.tasks.Task&gt; - 이 컬렉션의 [Task](../../com.aspose.tasks/task) 클래스 인스턴스를 포함하는 리스트를 반환합니다.
