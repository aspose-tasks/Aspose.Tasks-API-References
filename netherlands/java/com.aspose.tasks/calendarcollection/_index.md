---
title: "CalendarCollection"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een collectie van objecten voor."
type: docs
weight: 42
url: /nl/java/com.aspose.tasks/calendarcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class CalendarCollection extends AbstractList<Calendar>
```

Stelt een verzameling van [Calendar](../../com.aspose.tasks/calendar) objecten voor.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [add(String name)](#add-java.lang.String-) | Voegt een nieuwe basisagenda toe aan dit CalendarCollection-object en retourneert de toegevoegde agenda. |
| [add(String name, Calendar baseCalendar)](#add-java.lang.String-com.aspose.tasks.Calendar-) | Voegt een nieuwe agenda toe met de opgegeven basisagenda aan dit CalendarCollection-object en retourneert de toegevoegde agenda. |
| [clear()](#clear--) | Verwijdert alle elementen uit deze collectie. |
| [get(int index)](#get-int-) | (@inheritDoc\\} |
| [getByName(String name)](#getByName-java.lang.String-) | Retourneert een agenda met de opgegeven naam. |
| [getByUid(int uid)](#getByUid-int-) | Retourneert een agenda met de opgegeven UID. |
| [iterator()](#iterator--) | Retourneert een enumerator voor deze collectie. |
| [remove(int index)](#remove-int-) | Verwijdert het element op de opgegeven positie in deze lijst. |
| [remove(Object item)](#remove-java.lang.Object-) | Verwijdert Agenda uit de Project CalendarCollection. |
| [set(int index, Calendar element)](#set-int-com.aspose.tasks.Calendar-) | Vervangt het element op de opgegeven positie in deze lijst door het opgegeven element. |
| [size()](#size--) | Haalt het aantal objecten op dat in dit [CalendarCollection](../../com.aspose.tasks/calendarcollection)-object is opgenomen. |
| [toList()](#toList--) | Converteert het CalendarCollection-object naar een lijst van [Calendar](../../com.aspose.tasks/calendar)-objecten. |
### add(String name) {#add-java.lang.String-}
```
public final Calendar add(String name)
```


Voegt een nieuwe basisagenda toe aan dit CalendarCollection-object en retourneert de toegevoegde agenda.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String | Agenda-naam. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Added [Calendar](../../com.aspose.tasks/calendar) object.
### add(String name, Calendar baseCalendar) {#add-java.lang.String-com.aspose.tasks.Calendar-}
```
public final Calendar add(String name, Calendar baseCalendar)
```


Voegt een nieuwe agenda toe met de opgegeven basisagenda aan dit CalendarCollection-object en retourneert de toegevoegde agenda.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String | Opgegeven naam. |
| baseCalendar | [Calendar](../../com.aspose.tasks/calendar) | Opgegeven basisagenda. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Added [Calendar](../../com.aspose.tasks/calendar) object.
### clear() {#clear--}
```
public final void clear()
```


Verwijdert alle elementen uit deze collectie.

### get(int index) {#get-int-}
```
public Calendar get(int index)
```


(@inheritDoc\\}

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - \{@inheritDoc\}
### getByName(String name) {#getByName-java.lang.String-}
```
public final Calendar getByName(String name)
```


Retourneert een agenda met de opgegeven naam.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String | Naam van een agenda. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - If found returns calendar with a specified name else returns null.
### getByUid(int uid) {#getByUid-int-}
```
public final Calendar getByUid(int uid)
```


Retourneert een agenda met de opgegeven UID.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| uid | int | UID van een agenda. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Calendar with a specified UID.
### iterator() {#iterator--}
```
public Iterator<Calendar> iterator()
```


Retourneert een enumerator voor deze collectie.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Calendar&gt; - een enumerator voor deze collectie.
### remove(int index) {#remove-int-}
```
public Calendar remove(int index)
```


Verwijdert het element op de opgegeven positie in deze lijst.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - \{@inheritDoc\}
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


Verwijdert Agenda uit de Project CalendarCollection.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| item | java.lang.Object | De agenda om te verwijderen. |

**Returns:**
boolean - Als verwijderd, retourneert true, anders false.
### set(int index, Calendar element) {#set-int-com.aspose.tasks.Calendar-}
```
public Calendar set(int index, Calendar element)
```


Vervangt het element op de opgegeven positie in deze lijst door het opgegeven element.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |
| element | [Calendar](../../com.aspose.tasks/calendar) | \{@inheritDoc\} |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - \{@inheritDoc\}
### size() {#size--}
```
public final int size()
```


Haalt het aantal objecten op dat in dit [CalendarCollection](../../com.aspose.tasks/calendarcollection)-object is opgenomen.

**Returns:**
int - het aantal objecten dat in dit [CalendarCollection](../../com.aspose.tasks/calendarcollection)-object is opgenomen.
### toList() {#toList--}
```
public final List<Calendar> toList()
```


Converteert het CalendarCollection-object naar een lijst van [Calendar](../../com.aspose.tasks/calendar)-objecten.

**Returns:**
java.util.List&lt;com.aspose.tasks.Calendar&gt; - Lijst van [Calendar](../../com.aspose.tasks/calendar)-objecten.
