---
title: "CalendarCollection"
second_title: "Aspose.Tasks for Java API Reference"
description: "객체 컬렉션을 나타냅니다."
type: docs
weight: 42
url: /ko/java/com.aspose.tasks/calendarcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class CalendarCollection extends AbstractList<Calendar>
```

컬렉션은 [Calendar](../../com.aspose.tasks/calendar) 객체들의 모음입니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [add(String name)](#add-java.lang.String-) | 새 기본 캘린더를 이 CalendarCollection 객체에 추가하고 추가된 캘린더를 반환합니다. |
| [add(String name, Calendar baseCalendar)](#add-java.lang.String-com.aspose.tasks.Calendar-) | 지정된 기본 캘린더와 함께 새 캘린더를 이 CalendarCollection 객체에 추가하고 추가된 캘린더를 반환합니다. |
| [clear()](#clear--) | 이 컬렉션의 모든 요소를 제거합니다. |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getByName(String name)](#getByName-java.lang.String-) | 지정된 이름을 가진 캘린더를 반환합니다. |
| [getByUid(int uid)](#getByUid-int-) | 지정된 UID를 가진 캘린더를 반환합니다. |
| [iterator()](#iterator--) | 이 컬렉션에 대한 열거자를 반환합니다. |
| [remove(int index)](#remove-int-) | 이 목록에서 지정된 위치의 요소를 제거합니다. |
| [remove(Object item)](#remove-java.lang.Object-) | 프로젝트 CalendarCollection에서 캘린더를 제거합니다. |
| [set(int index, Calendar element)](#set-int-com.aspose.tasks.Calendar-) | 이 리스트의 지정된 위치에 있는 요소를 지정된 요소로 교체합니다. |
| [size()](#size--) | 이 [CalendarCollection](../../com.aspose.tasks/calendarcollection) 객체에 포함된 객체 수를 가져옵니다. |
| [toList()](#toList--) | CalendarCollection 객체를 [Calendar](../../com.aspose.tasks/calendar) 객체 목록으로 변환합니다. |
### add(String name) {#add-java.lang.String-}
```
public final Calendar add(String name)
```


새 기본 캘린더를 이 CalendarCollection 객체에 추가하고 추가된 캘린더를 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | java.lang.String | 캘린더 이름. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Added [Calendar](../../com.aspose.tasks/calendar) object.
### add(String name, Calendar baseCalendar) {#add-java.lang.String-com.aspose.tasks.Calendar-}
```
public final Calendar add(String name, Calendar baseCalendar)
```


지정된 기본 캘린더와 함께 새 캘린더를 이 CalendarCollection 객체에 추가하고 추가된 캘린더를 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | java.lang.String | 지정된 이름. |
| baseCalendar | [Calendar](../../com.aspose.tasks/calendar) | 지정된 기본 캘린더. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Added [Calendar](../../com.aspose.tasks/calendar) object.
### clear() {#clear--}
```
public final void clear()
```


이 컬렉션의 모든 요소를 제거합니다.

### get(int index) {#get-int-}
```
public Calendar get(int index)
```


(@inheritDoc\}

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - \{@inheritDoc\}
### getByName(String name) {#getByName-java.lang.String-}
```
public final Calendar getByName(String name)
```


지정된 이름을 가진 캘린더를 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| name | java.lang.String | 캘린더의 이름. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - If found returns calendar with a specified name else returns null.
### getByUid(int uid) {#getByUid-int-}
```
public final Calendar getByUid(int uid)
```


지정된 UID를 가진 캘린더를 반환합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| uid | int | 캘린더의 UID. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Calendar with a specified UID.
### iterator() {#iterator--}
```
public Iterator<Calendar> iterator()
```


이 컬렉션에 대한 열거자를 반환합니다.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Calendar&gt; - 이 컬렉션에 대한 열거자.
### remove(int index) {#remove-int-}
```
public Calendar remove(int index)
```


이 목록에서 지정된 위치의 요소를 제거합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - \{@inheritDoc\}
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


프로젝트 CalendarCollection에서 캘린더를 제거합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| item | java.lang.Object | 제거할 캘린더. |

**Returns:**
boolean - 제거되면 true를 반환하고, 그렇지 않으면 false를 반환합니다.
### set(int index, Calendar element) {#set-int-com.aspose.tasks.Calendar-}
```
public Calendar set(int index, Calendar element)
```


이 리스트의 지정된 위치에 있는 요소를 지정된 요소로 교체합니다.

**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |
| element | [Calendar](../../com.aspose.tasks/calendar) | \{@inheritDoc\} |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - \{@inheritDoc\}
### size() {#size--}
```
public final int size()
```


이 [CalendarCollection](../../com.aspose.tasks/calendarcollection) 객체에 포함된 객체 수를 가져옵니다.

**Returns:**
int - 이 [CalendarCollection](../../com.aspose.tasks/calendarcollection) 객체에 포함된 객체 수.
### toList() {#toList--}
```
public final List<Calendar> toList()
```


CalendarCollection 객체를 [Calendar](../../com.aspose.tasks/calendar) 객체 목록으로 변환합니다.

**Returns:**
java.util.List&lt;com.aspose.tasks.Calendar&gt; - [Calendar](../../com.aspose.tasks/calendar) 객체들의 목록.
