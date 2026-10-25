---
title: "CalendarCollection"
second_title: "Aspose.Tasks for Java API Reference"
description: "Rappresenta una raccolta di oggetti."
type: docs
weight: 42
url: /it/java/com.aspose.tasks/calendarcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class CalendarCollection extends AbstractList<Calendar>
```

Rappresenta una raccolta di oggetti [Calendar](../../com.aspose.tasks/calendar).
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [add(String name)](#add-java.lang.String-) | Aggiunge un nuovo calendario base a questo oggetto CalendarCollection e restituisce il calendario aggiunto. |
| [add(String name, Calendar baseCalendar)](#add-java.lang.String-com.aspose.tasks.Calendar-) | Aggiunge un nuovo calendario con il calendario base specificato a questo oggetto CalendarCollection e restituisce il calendario aggiunto. |
| [clear()](#clear--) | Rimuove tutti gli elementi da questa raccolta. |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getByName(String name)](#getByName-java.lang.String-) | Restituisce un calendario con il nome specificato. |
| [getByUid(int uid)](#getByUid-int-) | Restituisce un calendario con l'UID specificato. |
| [iterator()](#iterator--) | Restituisce un enumeratore per questa collezione. |
| [remove(int index)](#remove-int-) | Rimuove l'elemento nella posizione specificata in questo elenco. |
| [remove(Object item)](#remove-java.lang.Object-) | Rimuove Calendar dalla CalendarCollection del progetto. |
| [set(int index, Calendar element)](#set-int-com.aspose.tasks.Calendar-) | Sostituisce l'elemento nella posizione specificata in questa lista con l'elemento specificato. |
| [size()](#size--) | Ottiene il numero di oggetti contenuti in questo oggetto [CalendarCollection](../../com.aspose.tasks/calendarcollection). |
| [toList()](#toList--) | Converte l'oggetto CalendarCollection in un elenco di oggetti [Calendar](../../com.aspose.tasks/calendar). |
### add(String name) {#add-java.lang.String-}
```
public final Calendar add(String name)
```


Aggiunge un nuovo calendario base a questo oggetto CalendarCollection e restituisce il calendario aggiunto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Nome del calendario. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Added [Calendar](../../com.aspose.tasks/calendar) object.
### add(String name, Calendar baseCalendar) {#add-java.lang.String-com.aspose.tasks.Calendar-}
```
public final Calendar add(String name, Calendar baseCalendar)
```


Aggiunge un nuovo calendario con il calendario base specificato a questo oggetto CalendarCollection e restituisce il calendario aggiunto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Nome specificato. |
| baseCalendar | [Calendar](../../com.aspose.tasks/calendar) | Calendario base specificato. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Added [Calendar](../../com.aspose.tasks/calendar) object.
### clear() {#clear--}
```
public final void clear()
```


Rimuove tutti gli elementi da questa raccolta.

### get(int index) {#get-int-}
```
public Calendar get(int index)
```


(@inheritDoc\}

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - \{@inheritDoc\}
### getByName(String name) {#getByName-java.lang.String-}
```
public final Calendar getByName(String name)
```


Restituisce un calendario con il nome specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Nome di un calendario. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - If found returns calendar with a specified name else returns null.
### getByUid(int uid) {#getByUid-int-}
```
public final Calendar getByUid(int uid)
```


Restituisce un calendario con l'UID specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uid | int | UID di un calendario. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Calendar with a specified UID.
### iterator() {#iterator--}
```
public Iterator<Calendar> iterator()
```


Restituisce un enumeratore per questa collezione.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Calendar&gt; - un enumeratore per questa raccolta.
### remove(int index) {#remove-int-}
```
public Calendar remove(int index)
```


Rimuove l'elemento nella posizione specificata in questo elenco.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - \{@inheritDoc\}
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


Rimuove Calendar dalla CalendarCollection del progetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| elemento | java.lang.Object | Il calendario da rimuovere. |

**Returns:**
boolean - Se rimosso restituisce true, altrimenti restituisce false.
### set(int index, Calendar element) {#set-int-com.aspose.tasks.Calendar-}
```
public Calendar set(int index, Calendar element)
```


Sostituisce l'elemento nella posizione specificata in questa lista con l'elemento specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |
| element | [Calendar](../../com.aspose.tasks/calendar) | \{@inheritDoc\} |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - \{@inheritDoc\}
### size() {#size--}
```
public final int size()
```


Ottiene il numero di oggetti contenuti in questo oggetto [CalendarCollection](../../com.aspose.tasks/calendarcollection).

**Returns:**
int - il numero di oggetti contenuti in questo oggetto [CalendarCollection](../../com.aspose.tasks/calendarcollection).
### toList() {#toList--}
```
public final List<Calendar> toList()
```


Converte l'oggetto CalendarCollection in un elenco di oggetti [Calendar](../../com.aspose.tasks/calendar).

**Returns:**
java.util.List&lt;com.aspose.tasks.Calendar&gt; - Elenco di oggetti [Calendar](../../com.aspose.tasks/calendar).
