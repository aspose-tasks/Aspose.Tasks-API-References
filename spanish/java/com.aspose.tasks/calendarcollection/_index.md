---
title: "CalendarCollection"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa una colección de objetos."
type: docs
weight: 42
url: /es/java/com.aspose.tasks/calendarcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class CalendarCollection extends AbstractList<Calendar>
```

Representa una colección de objetos [Calendar](../../com.aspose.tasks/calendar).
## Métodos

| Método | Descripción |
| --- | --- |
| [add(String name)](#add-java.lang.String-) | Agrega un nuevo calendario base a este objeto CalendarCollection y devuelve el calendario agregado. |
| [add(String name, Calendar baseCalendar)](#add-java.lang.String-com.aspose.tasks.Calendar-) | Agrega un nuevo calendario con el calendario base especificado a este objeto CalendarCollection y devuelve el calendario agregado. |
| [clear()](#clear--) | Elimina todos los elementos de esta colección. |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getByName(String name)](#getByName-java.lang.String-) | Devuelve un calendario con el nombre especificado. |
| [getByUid(int uid)](#getByUid-int-) | Devuelve un calendario con el UID especificado. |
| [iterator()](#iterator--) | Devuelve un enumerador para esta colección. |
| [remove(int index)](#remove-int-) | Elimina el elemento en la posición especificada de esta lista. |
| [remove(Object item)](#remove-java.lang.Object-) | Elimina Calendar del CalendarCollection del proyecto. |
| [set(int index, Calendar element)](#set-int-com.aspose.tasks.Calendar-) | Reemplaza el elemento en la posición especificada de esta lista con el elemento especificado. |
| [size()](#size--) | Obtiene el número de objetos contenidos en este objeto [CalendarCollection](../../com.aspose.tasks/calendarcollection). |
| [toList()](#toList--) | Convierte el objeto CalendarCollection a una lista de objetos [Calendar](../../com.aspose.tasks/calendar). |
### add(String name) {#add-java.lang.String-}
```
public final Calendar add(String name)
```


Agrega un nuevo calendario base a este objeto CalendarCollection y devuelve el calendario agregado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | Nombre del calendario. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Added [Calendar](../../com.aspose.tasks/calendar) object.
### add(String name, Calendar baseCalendar) {#add-java.lang.String-com.aspose.tasks.Calendar-}
```
public final Calendar add(String name, Calendar baseCalendar)
```


Agrega un nuevo calendario con el calendario base especificado a este objeto CalendarCollection y devuelve el calendario agregado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | Nombre especificado. |
| baseCalendar | [Calendar](../../com.aspose.tasks/calendar) | Calendario base especificado. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Added [Calendar](../../com.aspose.tasks/calendar) object.
### clear() {#clear--}
```
public final void clear()
```


Elimina todos los elementos de esta colección.

### get(int index) {#get-int-}
```
public Calendar get(int index)
```


(@inheritDoc\}

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | \{@inheritDoc\} |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - \{@inheritDoc\}
### getByName(String name) {#getByName-java.lang.String-}
```
public final Calendar getByName(String name)
```


Devuelve un calendario con el nombre especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | Nombre de un calendario. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - If found returns calendar with a specified name else returns null.
### getByUid(int uid) {#getByUid-int-}
```
public final Calendar getByUid(int uid)
```


Devuelve un calendario con el UID especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| uid | int | UID de un calendario. |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - Calendar with a specified UID.
### iterator() {#iterator--}
```
public Iterator<Calendar> iterator()
```


Devuelve un enumerador para esta colección.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Calendar&gt; - un enumerador para esta colección.
### remove(int index) {#remove-int-}
```
public Calendar remove(int index)
```


Elimina el elemento en la posición especificada de esta lista.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | \{@inheritDoc\} |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - \{@inheritDoc\}
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


Elimina Calendar del CalendarCollection del proyecto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| elemento | java.lang.Object | El calendario a eliminar. |

**Returns:**
boolean - Si se elimina devuelve true, de lo contrario devuelve false.
### set(int index, Calendar element) {#set-int-com.aspose.tasks.Calendar-}
```
public Calendar set(int index, Calendar element)
```


Reemplaza el elemento en la posición especificada de esta lista con el elemento especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | int | \{@inheritDoc\} |
| element | [Calendar](../../com.aspose.tasks/calendar) | \{@inheritDoc\} |

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - \{@inheritDoc\}
### size() {#size--}
```
public final int size()
```


Obtiene el número de objetos contenidos en este objeto [CalendarCollection](../../com.aspose.tasks/calendarcollection).

**Returns:**
int - el número de objetos contenidos en este objeto [CalendarCollection](../../com.aspose.tasks/calendarcollection).
### toList() {#toList--}
```
public final List<Calendar> toList()
```


Convierte el objeto CalendarCollection a una lista de objetos [Calendar](../../com.aspose.tasks/calendar).

**Returns:**
java.util.List&lt;com.aspose.tasks.Calendar&gt; - Lista de objetos [Calendar](../../com.aspose.tasks/calendar).
