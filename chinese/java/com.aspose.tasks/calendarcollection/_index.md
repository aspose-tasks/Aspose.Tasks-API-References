---
title: "CalendarCollection"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示对象的集合。"
type: docs
weight: 42
url: /zh/java/com.aspose.tasks/calendarcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class CalendarCollection extends AbstractList<Calendar>
```

表示一个由 [Calendar](../../com.aspose.tasks/calendar) 对象组成的集合。
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(String name)](#add-java.lang.String-) | 向此 CalendarCollection 对象添加一个新的基础日历并返回添加的日历。 |
| [add(String name, Calendar baseCalendar)](#add-java.lang.String-com.aspose.tasks.Calendar-) | 向此 CalendarCollection 对象添加一个带有指定基础日历的新日历并返回添加的日历。 |
| [clear()](#clear--) | 从此集合中移除所有元素。 |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getByName(String name)](#getByName-java.lang.String-) | 返回具有指定名称的日历。 |
| [getByUid(int uid)](#getByUid-int-) | 返回具有指定 UID 的日历。 |
| [iterator()](#iterator--) | 返回此集合的枚举器。 |
| [remove(int index)](#remove-int-) | 移除此列表中指定位置的元素。 |
| [remove(Object item)](#remove-java.lang.Object-) | 从项目 CalendarCollection 中移除 Calendar。 |
| [set(int index, Calendar element)](#set-int-com.aspose.tasks.Calendar-) | 用指定的元素替换此列表中指定位置的元素。 |
| [size()](#size--) | 获取此 [CalendarCollection](../../com.aspose.tasks/calendarcollection) 对象中包含的对象数量。 |
| [toList()](#toList--) | 将 CalendarCollection 对象转换为 [Calendar](../../com.aspose.tasks/calendar) 对象的列表。 |
### add(String name) {#add-java.lang.String-}
```
public final Calendar add(String name)
```


向此 CalendarCollection 对象添加一个新的基础日历并返回添加的日历。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| name | java.lang.String | 日历名称。 |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Added [Calendar](../../com.aspose.tasks/calendar) object.
### add(String name, Calendar baseCalendar) {#add-java.lang.String-com.aspose.tasks.Calendar-}
```
public final Calendar add(String name, Calendar baseCalendar)
```


向此 CalendarCollection 对象添加一个带有指定基础日历的新日历并返回添加的日历。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| name | java.lang.String | 指定的名称。 |
| baseCalendar | [Calendar](../../com.aspose.tasks/calendar) | 指定的基础日历。 |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Added [Calendar](../../com.aspose.tasks/calendar) object.
### clear() {#clear--}
```
public final void clear()
```


从此集合中移除所有元素。

### get(int index) {#get-int-}
```
public Calendar get(int index)
```


(@inheritDoc\}

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | \{@inheritDoc\} |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - \{@inheritDoc\}
### getByName(String name) {#getByName-java.lang.String-}
```
public final Calendar getByName(String name)
```


返回具有指定名称的日历。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| name | java.lang.String | 日历的名称。 |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - If found returns calendar with a specified name else returns null.
### getByUid(int uid) {#getByUid-int-}
```
public final Calendar getByUid(int uid)
```


返回具有指定 UID 的日历。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| uid | int | 日历的 UID。 |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Calendar with a specified UID.
### iterator() {#iterator--}
```
public Iterator<Calendar> iterator()
```


返回此集合的枚举器。

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Calendar&gt; - 此集合的枚举器。
### remove(int index) {#remove-int-}
```
public Calendar remove(int index)
```


移除此列表中指定位置的元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | \{@inheritDoc\} |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - \{@inheritDoc\}
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


从项目 CalendarCollection 中移除 Calendar。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 项 | java.lang.Object | 要删除的日历。 |

**Returns:**
boolean - 如果已删除返回 true，否则返回 false。
### set(int index, Calendar element) {#set-int-com.aspose.tasks.Calendar-}
```
public Calendar set(int index, Calendar element)
```


用指定的元素替换此列表中指定位置的元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | \{@inheritDoc\} |
| element | [Calendar](../../com.aspose.tasks/calendar) | \{@inheritDoc\} |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - \{@inheritDoc\}
### size() {#size--}
```
public final int size()
```


获取此 [CalendarCollection](../../com.aspose.tasks/calendarcollection) 对象中包含的对象数量。

**Returns:**
int - 此 [CalendarCollection](../../com.aspose.tasks/calendarcollection) 对象中包含的对象数量。
### toList() {#toList--}
```
public final List<Calendar> toList()
```


将 CalendarCollection 对象转换为 [Calendar](../../com.aspose.tasks/calendar) 对象的列表。

**Returns:**
java.util.List&lt;com.aspose.tasks.Calendar&gt; - [Calendar](../../com.aspose.tasks/calendar) 对象的列表。
