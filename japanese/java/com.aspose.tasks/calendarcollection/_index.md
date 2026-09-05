---
title: "CalendarCollection"
second_title: "Aspose.Tasks for Java API リファレンス"
description: "オブジェクトのコレクションを表します。"
type: docs
weight: 42
url: /ja/java/com.aspose.tasks/calendarcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class CalendarCollection extends AbstractList<Calendar>
```

[Calendar](../../com.aspose/tasks/calendar) オブジェクトのコレクションを表します。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [add(String name)](#add-java.lang.String-) | この CalendarCollection オブジェクトに新しいベース カレンダーを追加し、追加されたカレンダーを返します。 |
| [add(String name, Calendar baseCalendar)](#add-java.lang.String-com.aspose.tasks.Calendar-) | この CalendarCollection オブジェクトに指定されたベース カレンダーを持つ新しいカレンダーを追加し、追加されたカレンダーを返します。 |
| [clear()](#clear--) | このコレクションからすべての要素を削除します。 |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getByName(String name)](#getByName-java.lang.String-) | 指定された名前のカレンダーを返します。 |
| [getByUid(int uid)](#getByUid-int-) | 指定された UID のカレンダーを返します。 |
| [iterator()](#iterator--) | このコレクションの列挙子を返します。 |
| [remove(int index)](#remove-int-) | このリストの指定された位置にある要素を削除します。 |
| [remove(Object item)](#remove-java.lang.Object-) | プロジェクトの CalendarCollection から Calendar を削除します。 |
| [set(int index, Calendar element)](#set-int-com.aspose.tasks.Calendar-) | このリストの指定された位置にある要素を、指定された要素に置き換えます。 |
| [size()](#size--) | この [CalendarCollection](../../com.aspose.tasks/calendarcollection) オブジェクトに含まれるオブジェクト数を取得します。 |
| [toList()](#toList--) | CalendarCollection オブジェクトを [Calendar](../../com.aspose.tasks/calendar) オブジェクトのリストに変換します。 |
### add(String name) {#add-java.lang.String-}
```
public final Calendar add(String name)
```


この CalendarCollection オブジェクトに新しいベース カレンダーを追加し、追加されたカレンダーを返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | java.lang.String | カレンダー名。 |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Added [Calendar](../../com.aspose.tasks/calendar) object.
### add(String name, Calendar baseCalendar) {#add-java.lang.String-com.aspose.tasks.Calendar-}
```
public final Calendar add(String name, Calendar baseCalendar)
```


この CalendarCollection オブジェクトに指定されたベース カレンダーを持つ新しいカレンダーを追加し、追加されたカレンダーを返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | java.lang.String | 指定された名前。 |
| baseCalendar | [Calendar](../../com.aspose.tasks/calendar) | 指定されたベースカレンダー。 |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Added [Calendar](../../com.aspose.tasks/calendar) object.
### clear() {#clear--}
```
public final void clear()
```


このコレクションからすべての要素を削除します。

### get(int index) {#get-int-}
```
public Calendar get(int index)
```


(@inheritDoc\}

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| インデックス | int | \{@inheritDoc\} |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - \{@inheritDoc\}
### getByName(String name) {#getByName-java.lang.String-}
```
public final Calendar getByName(String name)
```


指定された名前のカレンダーを返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| name | java.lang.String | カレンダーの名前。 |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - If found returns calendar with a specified name else returns null.
### getByUid(int uid) {#getByUid-int-}
```
public final Calendar getByUid(int uid)
```


指定された UID のカレンダーを返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| uid | int | カレンダーの UID。 |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Calendar with a specified UID.
### iterator() {#iterator--}
```
public Iterator<Calendar> iterator()
```


このコレクションの列挙子を返します。

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Calendar&gt; - このコレクションの列挙子。
### remove(int index) {#remove-int-}
```
public Calendar remove(int index)
```


このリストの指定された位置にある要素を削除します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| インデックス | int | \{@inheritDoc\} |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - \{@inheritDoc\}
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


プロジェクトの CalendarCollection から Calendar を削除します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| アイテム | java.lang.Object | 削除するカレンダー。 |

**Returns:**
boolean - 削除された場合は true、そうでない場合は false を返します。
### set(int index, Calendar element) {#set-int-com.aspose.tasks.Calendar-}
```
public Calendar set(int index, Calendar element)
```


このリストの指定された位置にある要素を、指定された要素に置き換えます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| インデックス | int | \{@inheritDoc\} |
| element | [Calendar](../../com.aspose.tasks/calendar) | \{@inheritDoc\} |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - \{@inheritDoc\}
### size() {#size--}
```
public final int size()
```


この [CalendarCollection](../../com.aspose.tasks/calendarcollection) オブジェクトに含まれるオブジェクト数を取得します。

**Returns:**
int - この [CalendarCollection](../../com.aspose.tasks/calendarcollection) オブジェクトに含まれるオブジェクトの数。
### toList() {#toList--}
```
public final List<Calendar> toList()
```


CalendarCollection オブジェクトを [Calendar](../../com.aspose.tasks/calendar) オブジェクトのリストに変換します。

**Returns:**
java.util.List&lt;com.aspose.tasks.Calendar&gt; - [Calendar](../../com.aspose.tasks/calendar) オブジェクトのリスト。
