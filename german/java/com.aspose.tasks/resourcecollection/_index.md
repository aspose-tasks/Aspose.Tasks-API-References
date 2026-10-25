---
title: "ResourceCollection"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt eine Sammlung von Objekten dar."
type: docs
weight: 251
url: /de/java/com.aspose.tasks/resourcecollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class ResourceCollection extends AbstractList<Resource>
```

Stellt eine Sammlung von [Resource](../../com.aspose.tasks/resource)-Objekten dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add()](#add--) | Fügt eine neue Ressource an der letzten Position einer Projektressourcen-Sammlung hinzu. |
| [add(Resource e)](#add-com.aspose.tasks.Resource-) | \{@inheritDoc\} |
| [add(String resourceName)](#add-java.lang.String-) | Fügt eine neue Ressource an der letzten Position einer Projektressourcen-Sammlung hinzu. |
| [add(String resourceName, int beforeResourceId)](#add-java.lang.String-int-) | Fügt eine neue Ressource an der angegebenen Position einer Projektressourcen-Sammlung hinzu. |
| [clear()](#clear--) | Direktes Leeren wird nicht unterstützt, diese Methode wirft lediglich eine UnsupportedOperationException. |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getById(int id)](#getById-int-) | Gibt eine Ressource mit der angegebenen ID zurück. |
| [getByUid(int uid)](#getByUid-int-) | Gibt eine Ressource mit dem angegebenen Uuid zurück. |
| [getParentProject()](#getParentProject--) | Ermittelt das übergeordnete Projekt des ResourceCollection-Objekts. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | \{@inheritDoc\} |
| [iterator()](#iterator--) | Gibt einen Enumerator für diese Sammlung zurück. |
| [remove(Object o)](#remove-java.lang.Object-) | Dies ist die Stub-Implementierung der remove-Methode von Collection, die nur eine UnsupportedOperationException wirft. |
| [size()](#size--) | Ermittelt die Anzahl der im ResourceCollection enthaltenen Elemente. |
| [sort(Comparator&lt;? super Resource&gt; comparer)](#sort-java.util.Comparator---super-com.aspose.tasks.Resource--) | \{@inheritDoc\} |
| [toList()](#toList--) | Konvertiert das ResourceCollection-Objekt in eine Liste von [Resource](../../com.aspose.tasks/resource)-Objekten. |
### add() {#add--}
```
public final Resource add()
```


Fügt eine neue Ressource an der letzten Position einer Projektressourcen-Sammlung hinzu.

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### add(Resource e) {#add-com.aspose.tasks.Resource-}
```
public final boolean add(Resource e)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| e | [Resource](../../com.aspose.tasks/resource) | \{@inheritDoc\} |

**Returns:**
boolean - \\{@inheritDoc\\}
### add(String resourceName) {#add-java.lang.String-}
```
public final Resource add(String resourceName)
```


Fügt eine neue Ressource an der letzten Position einer Projektressourcen-Sammlung hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| resourceName | java.lang.String | Name einer Ressource. |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### add(String resourceName, int beforeResourceId) {#add-java.lang.String-int-}
```
public final Resource add(String resourceName, int beforeResourceId)
```


Fügt eine neue Ressource an der angegebenen Position einer Projektressourcen-Sammlung hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| resourceName | java.lang.String | Name einer Ressource. |
| beforeResourceId | int | Position der vorherigen Ressource in einer Projektressourcen-Sammlung. |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### clear() {#clear--}
```
public final void clear()
```


Direktes Leeren wird nicht unterstützt, diese Methode wirft lediglich eine UnsupportedOperationException.

### contains(Object o) {#contains-java.lang.Object-}
```
public final boolean contains(Object o)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \\{@inheritDoc\\}
### get(int index) {#get-int-}
```
public Resource get(int index)
```


(@inheritDoc\}

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | \{@inheritDoc\} |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - \{@inheritDoc\}
### getById(int id) {#getById-int-}
```
public final Resource getById(int id)
```


Gibt eine Ressource mit der angegebenen ID zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | ID | int | Die angegebene ID. |

--------------------

O(1)-Komplexität. |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Resource with the specified id if present; otherwise, null.
### getByUid(int uid) {#getByUid-int-}
```
public final Resource getByUid(int uid)
```


Gibt eine Ressource mit dem angegebenen Uuid zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | uid | int | Die angegebene UID. |

--------------------

O(1)-Komplexität. |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Resource with the specified uid if present; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Ermittelt das übergeordnete Projekt des ResourceCollection-Objekts.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the ResourceCollection object.
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public final int indexOf(Object o)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
int - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```




**Returns:**
boolean - \\{@inheritDoc\\}
### iterator() {#iterator--}
```
public final Iterator<Resource> iterator()
```


Gibt einen Enumerator für diese Sammlung zurück.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Resource&gt; - ein Enumerator für diese Sammlung.
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```


Dies ist die Stub-Implementierung der remove-Methode von Collection, die nur eine UnsupportedOperationException wirft.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | Das zu entfernende Element. |

**Returns:**
boolean - `true`, wenn das Element entfernt wurde; `false` andernfalls.
### size() {#size--}
```
public final int size()
```


Ermittelt die Anzahl der im ResourceCollection enthaltenen Elemente.

--------------------

Nur-Lese-`int`.

**Returns:**
int - die Anzahl der im ResourceCollection enthaltenen Elemente.
### sort(Comparator&lt;? super Resource&gt; comparer) {#sort-java.util.Comparator---super-com.aspose.tasks.Resource--}
```
public final void sort(Comparator<? super Resource> comparer)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| comparer | java.util.Comparator&lt;? super com.aspose.tasks.Resource&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<Resource> toList()
```


Konvertiert das ResourceCollection-Objekt in eine Liste von [Resource](../../com.aspose.tasks/resource)-Objekten.

**Returns:**
java.util.List&lt;com.aspose.tasks.Resource&gt; - Liste von [Resource](../../com.aspose.tasks/resource)-Objekten.
