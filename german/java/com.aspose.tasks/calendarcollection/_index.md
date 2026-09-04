---
title: "CalendarCollection"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt eine Sammlung von Objekten dar."
type: docs
weight: 42
url: /de/java/com.aspose.tasks/calendarcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class CalendarCollection extends AbstractList<Calendar>
```

Stellt eine Sammlung von [Calendar](../../com.aspose.tasks/calendar)-Objekten dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add(String name)](#add-java.lang.String-) | Fügt diesem CalendarCollection-Objekt einen neuen Basiskalender hinzu und gibt den hinzugefügten Kalender zurück. |
| [add(String name, Calendar baseCalendar)](#add-java.lang.String-com.aspose.tasks.Calendar-) | Fügt diesem CalendarCollection-Objekt einen neuen Kalender mit dem angegebenen Basiskalender hinzu und gibt den hinzugefügten Kalender zurück. |
| [clear()](#clear--) | Entfernt alle Elemente aus dieser Sammlung. |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getByName(String name)](#getByName-java.lang.String-) | Gibt einen Kalender mit dem angegebenen Namen zurück. |
| [getByUid(int uid)](#getByUid-int-) | Gibt einen Kalender mit der angegebenen UID zurück. |
| [iterator()](#iterator--) | Gibt einen Enumerator für diese Sammlung zurück. |
| [remove(int index)](#remove-int-) | Entfernt das Element an der angegebenen Position in dieser Liste. |
| [remove(Object item)](#remove-java.lang.Object-) | Entfernt Calendar aus Project CalendarCollection. |
| [set(int index, Calendar element)](#set-int-com.aspose.tasks.Calendar-) | Ersetzt das Element an der angegebenen Position in dieser Liste durch das angegebene Element. |
| [size()](#size--) | Ermittelt die Anzahl der in diesem [CalendarCollection](../../com.aspose.tasks/calendarcollection)-Objekt enthaltenen Objekte. |
| [toList()](#toList--) | Konvertiert das CalendarCollection-Objekt in eine Liste von [Calendar](../../com.aspose.tasks/calendar)-Objekten. |
### add(String name) {#add-java.lang.String-}
```
public final Calendar add(String name)
```


Fügt diesem CalendarCollection-Objekt einen neuen Basiskalender hinzu und gibt den hinzugefügten Kalender zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | java.lang.String | Calendar-Name. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Added [Calendar](../../com.aspose.tasks/calendar) object.
### add(String name, Calendar baseCalendar) {#add-java.lang.String-com.aspose.tasks.Calendar-}
```
public final Calendar add(String name, Calendar baseCalendar)
```


Fügt diesem CalendarCollection-Objekt einen neuen Kalender mit dem angegebenen Basiskalender hinzu und gibt den hinzugefügten Kalender zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | java.lang.String | Angegebener Name. |
| baseCalendar | [Calendar](../../com.aspose.tasks/calendar) | Angegebener Basiskalender. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Added [Calendar](../../com.aspose.tasks/calendar) object.
### clear() {#clear--}
```
public final void clear()
```


Entfernt alle Elemente aus dieser Sammlung.

### get(int index) {#get-int-}
```
public Calendar get(int index)
```


(@inheritDoc\}

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | \{@inheritDoc\} |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - \{@inheritDoc\}
### getByName(String name) {#getByName-java.lang.String-}
```
public final Calendar getByName(String name)
```


Gibt einen Kalender mit dem angegebenen Namen zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| name | java.lang.String | Name eines Kalenders. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - If found returns calendar with a specified name else returns null.
### getByUid(int uid) {#getByUid-int-}
```
public final Calendar getByUid(int uid)
```


Gibt einen Kalender mit der angegebenen UID zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| uid | int | UID eines Kalenders. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Calendar with a specified UID.
### iterator() {#iterator--}
```
public Iterator<Calendar> iterator()
```


Gibt einen Enumerator für diese Sammlung zurück.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Calendar&gt; - ein Enumerator für diese Sammlung.
### remove(int index) {#remove-int-}
```
public Calendar remove(int index)
```


Entfernt das Element an der angegebenen Position in dieser Liste.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | \{@inheritDoc\} |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - \{@inheritDoc\}
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


Entfernt Calendar aus Project CalendarCollection.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Element | java.lang.Object | Der zu entfernende Kalender. |

**Returns:**
boolean - Gibt true zurück, wenn entfernt, sonst false.
### set(int index, Calendar element) {#set-int-com.aspose.tasks.Calendar-}
```
public Calendar set(int index, Calendar element)
```


Ersetzt das Element an der angegebenen Position in dieser Liste durch das angegebene Element.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | \{@inheritDoc\} |
| element | [Calendar](../../com.aspose.tasks/calendar) | \{@inheritDoc\} |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - \{@inheritDoc\}
### size() {#size--}
```
public final int size()
```


Ermittelt die Anzahl der in diesem [CalendarCollection](../../com.aspose.tasks/calendarcollection)-Objekt enthaltenen Objekte.

**Returns:**
int - die Anzahl der Objekte, die in diesem [CalendarCollection](../../com.aspose.tasks/calendarcollection)-Objekt enthalten sind.
### toList() {#toList--}
```
public final List<Calendar> toList()
```


Konvertiert das CalendarCollection-Objekt in eine Liste von [Calendar](../../com.aspose.tasks/calendar)-Objekten.

**Returns:**
java.util.List&lt;com.aspose.tasks.Calendar&gt; - Liste von [Calendar](../../com.aspose.tasks/calendar)-Objekten.
