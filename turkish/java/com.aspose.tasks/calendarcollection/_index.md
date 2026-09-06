---
title: "CalendarCollection"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Nesnelerden oluşan bir koleksiyonu temsil eder."
type: docs
weight: 42
url: /tr/java/com.aspose.tasks/calendarcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class CalendarCollection extends AbstractList<Calendar>
```

Bir [Calendar](../../com.aspose.tasks/calendar) nesnesi koleksiyonunu temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(String name)](#add-java.lang.String-) | Bu CalendarCollection nesnesine yeni bir temel takvim ekler ve eklenen takvimi döndürür. |
| [add(String name, Calendar baseCalendar)](#add-java.lang.String-com.aspose.tasks.Calendar-) | Bu CalendarCollection nesnesine belirtilen temel takvimle yeni bir takvim ekler ve eklenen takvimi döndürür. |
| [clear()](#clear--) | Bu koleksiyondaki tüm öğeleri kaldırır. |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getByName(String name)](#getByName-java.lang.String-) | Belirtilen ada sahip bir takvim döndürür. |
| [getByUid(int uid)](#getByUid-int-) | Belirtilen UID'ye sahip bir takvim döndürür. |
| [iterator()](#iterator--) | Bu koleksiyon için bir enumerator döndürür. |
| [remove(int index)](#remove-int-) | Bu listedeki belirtilen konumdaki öğeyi kaldırır. |
| [remove(Object item)](#remove-java.lang.Object-) | Calendar'ı Proje CalendarCollection'dan kaldırır. |
| [set(int index, Calendar element)](#set-int-com.aspose.tasks.Calendar-) | Bu listedeki belirtilen konumdaki öğeyi belirtilen öğeyle değiştirir. |
| [size()](#size--) | Bu [CalendarCollection](../../com.aspose.tasks/calendarcollection) nesnesinde bulunan nesne sayısını alır. |
| [toList()](#toList--) | CalendarCollection nesnesini bir [Calendar](../../com.aspose.tasks/calendar) nesnesi listesine dönüştürür. |
### add(String name) {#add-java.lang.String-}
```
public final Calendar add(String name)
```


Bu CalendarCollection nesnesine yeni bir temel takvim ekler ve eklenen takvimi döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | java.lang.String | Takvim adı. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Added [Calendar](../../com.aspose.tasks/calendar) object.
### add(String name, Calendar baseCalendar) {#add-java.lang.String-com.aspose.tasks.Calendar-}
```
public final Calendar add(String name, Calendar baseCalendar)
```


Bu CalendarCollection nesnesine belirtilen temel takvimle yeni bir takvim ekler ve eklenen takvimi döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | java.lang.String | Belirtilen ad. |
| baseCalendar | [Calendar](../../com.aspose.tasks/calendar) | Belirtilen temel takvim. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Added [Calendar](../../com.aspose.tasks/calendar) object.
### clear() {#clear--}
```
public final void clear()
```


Bu koleksiyondaki tüm öğeleri kaldırır.

### get(int index) {#get-int-}
```
public Calendar get(int index)
```


(@inheritDoc\}

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - \{@inheritDoc\}
### getByName(String name) {#getByName-java.lang.String-}
```
public final Calendar getByName(String name)
```


Belirtilen ada sahip bir takvim döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | java.lang.String | Bir takvimin adı. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - If found returns calendar with a specified name else returns null.
### getByUid(int uid) {#getByUid-int-}
```
public final Calendar getByUid(int uid)
```


Belirtilen UID'ye sahip bir takvim döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| uid | int | Bir takvimin UID'si. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Calendar with a specified UID.
### iterator() {#iterator--}
```
public Iterator<Calendar> iterator()
```


Bu koleksiyon için bir enumerator döndürür.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Calendar&gt; - bu koleksiyon için bir yineleyici.
### remove(int index) {#remove-int-}
```
public Calendar remove(int index)
```


Bu listedeki belirtilen konumdaki öğeyi kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - \{@inheritDoc\}
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


Calendar'ı Proje CalendarCollection'dan kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| öğe | java.lang.Object | Kaldırılacak takvim. |

**Returns:**
boolean - Kaldırıldıysa true, aksi takdirde false döndürür.
### set(int index, Calendar element) {#set-int-com.aspose.tasks.Calendar-}
```
public Calendar set(int index, Calendar element)
```


Bu listedeki belirtilen konumdaki öğeyi belirtilen öğeyle değiştirir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |
| element | [Calendar](../../com.aspose.tasks/calendar) | \{@inheritDoc\} |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - \{@inheritDoc\}
### size() {#size--}
```
public final int size()
```


Bu [CalendarCollection](../../com.aspose.tasks/calendarcollection) nesnesinde bulunan nesne sayısını alır.

**Returns:**
int - bu [CalendarCollection](../../com.aspose.tasks/calendarcollection) nesnesinde bulunan nesne sayısı.
### toList() {#toList--}
```
public final List<Calendar> toList()
```


CalendarCollection nesnesini bir [Calendar](../../com.aspose.tasks/calendar) nesnesi listesine dönüştürür.

**Returns:**
java.util.List&lt;com.aspose.tasks.Calendar&gt; - [Calendar](../../com.aspose.tasks/calendar) nesnelerinin listesi.
