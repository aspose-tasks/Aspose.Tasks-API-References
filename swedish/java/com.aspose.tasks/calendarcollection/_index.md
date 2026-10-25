---
title: "CalendarCollection"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar en samling av  objekt."
type: docs
weight: 42
url: /sv/java/com.aspose.tasks/calendarcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class CalendarCollection extends AbstractList<Calendar>
```

Representerar en samling av [Calendar](../../com.aspose.tasks/calendar) objekt.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(String name)](#add-java.lang.String-) | Lägger till en ny grundkalender i detta CalendarCollection-objekt och returnerar den tillagda kalendern. |
| [add(String name, Calendar baseCalendar)](#add-java.lang.String-com.aspose.tasks.Calendar-) | Lägger till en ny kalender med angiven grundkalender i detta CalendarCollection-objekt och returnerar den tillagda kalendern. |
| [clear()](#clear--) | Tar bort alla element från denna samling. |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getByName(String name)](#getByName-java.lang.String-) | Returnerar en kalender med det angivna namnet. |
| [getByUid(int uid)](#getByUid-int-) | Returnerar en kalender med den angivna UID:n. |
| [iterator()](#iterator--) | Returnerar en enumerator för denna samling. |
| [remove(int index)](#remove-int-) | Tar bort elementet på den angivna positionen i denna lista. |
| [remove(Object item)](#remove-java.lang.Object-) | Tar bort Calendar från Project CalendarCollection. |
| [set(int index, Calendar element)](#set-int-com.aspose.tasks.Calendar-) | Ersätter elementet på den angivna positionen i denna lista med det angivna elementet. |
| [size()](#size--) | Hämtar antalet objekt som finns i detta [CalendarCollection](../../com.aspose.tasks/calendarcollection)-objekt. |
| [toList()](#toList--) | Konverterar CalendarCollection-objektet till en lista av [Calendar](../../com.aspose.tasks/calendar) objekt. |
### add(String name) {#add-java.lang.String-}
```
public final Calendar add(String name)
```


Lägger till en ny grundkalender i detta CalendarCollection-objekt och returnerar den tillagda kalendern.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Kalendernamn. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Added [Calendar](../../com.aspose.tasks/calendar) object.
### add(String name, Calendar baseCalendar) {#add-java.lang.String-com.aspose.tasks.Calendar-}
```
public final Calendar add(String name, Calendar baseCalendar)
```


Lägger till en ny kalender med angiven grundkalender i detta CalendarCollection-objekt och returnerar den tillagda kalendern.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Angivet namn. |
| baseCalendar | [Calendar](../../com.aspose.tasks/calendar) | Angiven grundkalender. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Added [Calendar](../../com.aspose.tasks/calendar) object.
### clear() {#clear--}
```
public final void clear()
```


Tar bort alla element från denna samling.

### get(int index) {#get-int-}
```
public Calendar get(int index)
```


(@inheritDoc\}

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - \{@inheritDoc\}
### getByName(String name) {#getByName-java.lang.String-}
```
public final Calendar getByName(String name)
```


Returnerar en kalender med det angivna namnet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Namn på en kalender. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - If found returns calendar with a specified name else returns null.
### getByUid(int uid) {#getByUid-int-}
```
public final Calendar getByUid(int uid)
```


Returnerar en kalender med den angivna UID:n.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| uid | int | UID för en kalender. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Calendar with a specified UID.
### iterator() {#iterator--}
```
public Iterator<Calendar> iterator()
```


Returnerar en enumerator för denna samling.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Calendar&gt; - en enumerator för denna samling.
### remove(int index) {#remove-int-}
```
public Calendar remove(int index)
```


Tar bort elementet på den angivna positionen i denna lista.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - \{@inheritDoc\}
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


Tar bort Calendar från Project CalendarCollection.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| objekt | java.lang.Object | Kalendern att ta bort. |

**Returns:**
boolean - Om den tas bort returneras true, annars false.
### set(int index, Calendar element) {#set-int-com.aspose.tasks.Calendar-}
```
public Calendar set(int index, Calendar element)
```


Ersätter elementet på den angivna positionen i denna lista med det angivna elementet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |
| element | [Calendar](../../com.aspose.tasks/calendar) | \{@inheritDoc\} |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - \{@inheritDoc\}
### size() {#size--}
```
public final int size()
```


Hämtar antalet objekt som finns i detta [CalendarCollection](../../com.aspose.tasks/calendarcollection)-objekt.

**Returns:**
int - antalet objekt som finns i detta [CalendarCollection](../../com.aspose.tasks/calendarcollection) objekt.
### toList() {#toList--}
```
public final List<Calendar> toList()
```


Konverterar CalendarCollection-objektet till en lista av [Calendar](../../com.aspose.tasks/calendar) objekt.

**Returns:**
java.util.List&lt;com.aspose.tasks.Calendar&gt; - Lista med [Calendar](../../com.aspose.tasks/calendar) objekt.
