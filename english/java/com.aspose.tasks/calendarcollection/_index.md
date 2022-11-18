---
title: CalendarCollection
second_title: Aspose.Tasks for Java API Reference
description: Represents a collection of  objects.
type: docs
weight: 42
url: /java/com.aspose.tasks/calendarcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class CalendarCollection extends AbstractList<Calendar>
```

Represents a collection of [Calendar](../../com.aspose.tasks/calendar) objects.
## Methods

| Method | Description |
| --- | --- |
| [add(String name)](#add-java.lang.String-) | Adds a new base calendar to this CalendarCollection object and returns added calendar. |
| [add(String name, Calendar baseCalendar)](#add-java.lang.String-com.aspose.tasks.Calendar-) | Adds a new calendar with specified base calendar to this CalendarCollection object and returns added calendar. |
| [clear()](#clear--) | Removes all of the elements from this collection. |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getByName(String name)](#getByName-java.lang.String-) | Returns a calendar with the specified name. |
| [getByUid(int uid)](#getByUid-int-) | Returns a calendar with the specified UID. |
| [getParentProject()](#getParentProject--) | Gets a parent [Project](../../com.aspose.tasks/project) of this object. |
| [iterator()](#iterator--) | Returns an enumerator for this collection. |
| [remove(int index)](#remove-int-) | Removes the element at the specified position in this list. |
| [remove(Object item)](#remove-java.lang.Object-) | Removes Calendar from Project CalendarCollection. |
| [set(int index, Calendar element)](#set-int-com.aspose.tasks.Calendar-) | Replaces the element at the specified position in this list with the specified element. |
| [size()](#size--) | Gets the number of objects contained in this [CalendarCollection](../../com.aspose.tasks/calendarcollection) object. |
| [toList()](#toList--) | Converts the CalendarCollection object to a list of [Calendar](../../com.aspose.tasks/calendar) objects. |
### add(String name) {#add-java.lang.String-}
```
public final Calendar add(String name)
```


Adds a new base calendar to this CalendarCollection object and returns added calendar.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Calendar name. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Added [Calendar](../../com.aspose.tasks/calendar) object.
### add(String name, Calendar baseCalendar) {#add-java.lang.String-com.aspose.tasks.Calendar-}
```
public final Calendar add(String name, Calendar baseCalendar)
```


Adds a new calendar with specified base calendar to this CalendarCollection object and returns added calendar.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Specified name. |
| baseCalendar | [Calendar](../../com.aspose.tasks/calendar) | Specified base calendar. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Added [Calendar](../../com.aspose.tasks/calendar) object.
### clear() {#clear--}
```
public final void clear()
```


Removes all of the elements from this collection.

### get(int index) {#get-int-}
```
public Calendar get(int index)
```


(@inheritDoc\}

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - \{@inheritDoc\}
### getByName(String name) {#getByName-java.lang.String-}
```
public final Calendar getByName(String name)
```


Returns a calendar with the specified name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String | Name of a calendar. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - If found returns calendar with a specified name else returns null.
### getByUid(int uid) {#getByUid-int-}
```
public final Calendar getByUid(int uid)
```


Returns a calendar with the specified UID.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| uid | int | UID of a calendar. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Calendar with a specified UID.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Gets a parent [Project](../../com.aspose.tasks/project) of this object.

**Returns:**
[Project](../../com.aspose.tasks/project) - a parent [Project](../../com.aspose.tasks/project) of this object.
### iterator() {#iterator--}
```
public Iterator<Calendar> iterator()
```


Returns an enumerator for this collection.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Calendar&gt; - an enumerator for this collection.
### remove(int index) {#remove-int-}
```
public Calendar remove(int index)
```


Removes the element at the specified position in this list.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - \{@inheritDoc\}
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


Removes Calendar from Project CalendarCollection.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| item | java.lang.Object | The calendar to remove. |

**Returns:**
boolean - If removed returns true, else returns false.
### set(int index, Calendar element) {#set-int-com.aspose.tasks.Calendar-}
```
public Calendar set(int index, Calendar element)
```


Replaces the element at the specified position in this list with the specified element.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |
| element | [Calendar](../../com.aspose.tasks/calendar) | \{@inheritDoc\} |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - \{@inheritDoc\}
### size() {#size--}
```
public final int size()
```


Gets the number of objects contained in this [CalendarCollection](../../com.aspose.tasks/calendarcollection) object.

**Returns:**
int - the number of objects contained in this [CalendarCollection](../../com.aspose.tasks/calendarcollection) object.
### toList() {#toList--}
```
public final List<Calendar> toList()
```


Converts the CalendarCollection object to a list of [Calendar](../../com.aspose.tasks/calendar) objects.

**Returns:**
java.util.List&lt;com.aspose.tasks.Calendar&gt; - List of [Calendar](../../com.aspose.tasks/calendar) objects.
