---
title: "CalendarCollection"
second_title: "مرجع API لـ Aspose.Tasks for Java"
description: "يمثل مجموعة من الكائنات."
type: docs
weight: 42
url: /ar/java/com.aspose.tasks/calendarcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class CalendarCollection extends AbstractList<Calendar>
```

يمثل مجموعة من كائنات [Calendar](../../com.aspose.tasks/calendar).
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(String name)](#add-java.lang.String-) | يضيف تقويمًا أساسيًا جديدًا إلى كائن CalendarCollection هذا ويعيد التقويم المضاف. |
| [add(String name, Calendar baseCalendar)](#add-java.lang.String-com.aspose.tasks.Calendar-) | يضيف تقويمًا جديدًا مع تقويم أساسي محدد إلى كائن CalendarCollection هذا ويعيد التقويم المضاف. |
| [clear()](#clear--) | يزيل جميع العناصر من هذه المجموعة. |
| [get(int index)](#get-int-) | (@inheritDoc\\} |
| [getByName(String name)](#getByName-java.lang.String-) | يعيد تقويمًا بالاسم المحدد. |
| [getByUid(int uid)](#getByUid-int-) | يعيد تقويمًا بالمعرف الفريد المحدد. |
| [iterator()](#iterator--) | يرجع مُعدِّدًا لهذه المجموعة. |
| [remove(int index)](#remove-int-) | يزيل العنصر في الموضع المحدد في هذه القائمة. |
| [remove(Object item)](#remove-java.lang.Object-) | يزيل Calendar من مجموعة CalendarCollection للمشروع. |
| [set(int index, Calendar element)](#set-int-com.aspose.tasks.Calendar-) | يستبدل العنصر في الموضع المحدد في هذه القائمة بالعنصر المحدد. |
| [size()](#size--) | يحصل على عدد الكائنات الموجودة في كائن [CalendarCollection](../../com.aspose.tasks/calendarcollection) هذا. |
| [toList()](#toList--) | يحوّل كائن CalendarCollection إلى قائمة من كائنات [Calendar](../../com.aspose.tasks/calendar). |
### add(String name) {#add-java.lang.String-}
```
public final Calendar add(String name)
```


يضيف تقويمًا أساسيًا جديدًا إلى كائن CalendarCollection هذا ويعيد التقويم المضاف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم التقويم. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Added [Calendar](../../com.aspose.tasks/calendar) object.
### add(String name, Calendar baseCalendar) {#add-java.lang.String-com.aspose.tasks.Calendar-}
```
public final Calendar add(String name, Calendar baseCalendar)
```


يضيف تقويمًا جديدًا مع تقويم أساسي محدد إلى كائن CalendarCollection هذا ويعيد التقويم المضاف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | الاسم المحدد. |
| baseCalendar | [Calendar](../../com.aspose.tasks/calendar) | التقويم الأساسي المحدد. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Added [Calendar](../../com.aspose.tasks/calendar) object.
### clear() {#clear--}
```
public final void clear()
```


يزيل جميع العناصر من هذه المجموعة.

### get(int index) {#get-int-}
```
public Calendar get(int index)
```


(@inheritDoc\\}

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | int | \{@inheritDoc\} |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - \{@inheritDoc\}
### getByName(String name) {#getByName-java.lang.String-}
```
public final Calendar getByName(String name)
```


يعيد تقويمًا بالاسم المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم التقويم. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - If found returns calendar with a specified name else returns null.
### getByUid(int uid) {#getByUid-int-}
```
public final Calendar getByUid(int uid)
```


يعيد تقويمًا بالمعرف الفريد المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| uid | int | UID للتقويم. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Calendar with a specified UID.
### iterator() {#iterator--}
```
public Iterator<Calendar> iterator()
```


يرجع مُعدِّدًا لهذه المجموعة.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Calendar&gt; - عداد لهذه المجموعة.
### remove(int index) {#remove-int-}
```
public Calendar remove(int index)
```


يزيل العنصر في الموضع المحدد في هذه القائمة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | int | \{@inheritDoc\} |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - \{@inheritDoc\}
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


يزيل Calendar من مجموعة CalendarCollection للمشروع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عنصر | java.lang.Object | التقويم المراد إزالته. |

**Returns:**
boolean - إذا تم الإزالة تُعيد true، وإلا تُعيد false.
### set(int index, Calendar element) {#set-int-com.aspose.tasks.Calendar-}
```
public Calendar set(int index, Calendar element)
```


يستبدل العنصر في الموضع المحدد في هذه القائمة بالعنصر المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | int | \{@inheritDoc\} |
| element | [Calendar](../../com.aspose.tasks/calendar) | \{@inheritDoc\} |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - \{@inheritDoc\}
### size() {#size--}
```
public final int size()
```


يحصل على عدد الكائنات الموجودة في كائن [CalendarCollection](../../com.aspose.tasks/calendarcollection) هذا.

**Returns:**
int - عدد الكائنات الموجودة في كائن [CalendarCollection](../../com.aspose.tasks/calendarcollection) هذا.
### toList() {#toList--}
```
public final List<Calendar> toList()
```


يحوّل كائن CalendarCollection إلى قائمة من كائنات [Calendar](../../com.aspose.tasks/calendar).

**Returns:**
java.util.List&lt;com.aspose.tasks.Calendar&gt; - قائمة من كائنات [Calendar](../../com.aspose.tasks/calendar).
