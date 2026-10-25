---
title: "ResourceCollection"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar en samling av  objekt."
type: docs
weight: 251
url: /sv/java/com.aspose.tasks/resourcecollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class ResourceCollection extends AbstractList<Resource>
```

Representerar en samling av [Resource](../../com.aspose.tasks/resource) objekt.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add()](#add--) | Lägger till en ny resurs på den sista positionen i en projekts resurskollektion. |
| [add(Resource e)](#add-com.aspose.tasks.Resource-) | \{@inheritDoc\} |
| [add(String resourceName)](#add-java.lang.String-) | Lägger till en ny resurs på den sista positionen i en projekts resurskollektion. |
| [add(String resourceName, int beforeResourceId)](#add-java.lang.String-int-) | Lägger till en ny resurs på den angivna positionen i en projekts resurskollektion. |
| [clear()](#clear--) | Direkt rensning stöds inte, den här metoden kastar bara UnsupportedOperationException. |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getById(int id)](#getById-int-) | Returnerar en resurs med det angivna id:t. |
| [getByUid(int uid)](#getByUid-int-) | Returnerar en resurs med den angivna Uid:n. |
| [getParentProject()](#getParentProject--) | Hämtar föräldraprojektet för ResourceCollection-objektet. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | \{@inheritDoc\} |
| [iterator()](#iterator--) | Returnerar en enumerator för denna samling. |
| [remove(Object o)](#remove-java.lang.Object-) | Detta är stub-implementationen av Collections remove‑metod, som bara kastar UnsupportedOperationException. |
| [size()](#size--) | Hämtar antalet element som finns i ResourceCollection. |
| [sort(Comparator&lt;? super Resource&gt; comparer)](#sort-java.util.Comparator---super-com.aspose.tasks.Resource--) | \{@inheritDoc\} |
| [toList()](#toList--) | Konverterar ResourceCollection-objektet till en lista av [Resource](../../com.aspose.tasks/resource) objekt. |
### add() {#add--}
```
public final Resource add()
```


Lägger till en ny resurs på den sista positionen i en projekts resurskollektion.

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### add(Resource e) {#add-com.aspose.tasks.Resource-}
```
public final boolean add(Resource e)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| e | [Resource](../../com.aspose.tasks/resource) | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### add(String resourceName) {#add-java.lang.String-}
```
public final Resource add(String resourceName)
```


Lägger till en ny resurs på den sista positionen i en projekts resurskollektion.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| resourceName | java.lang.String | Namn på en resurs. |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### add(String resourceName, int beforeResourceId) {#add-java.lang.String-int-}
```
public final Resource add(String resourceName, int beforeResourceId)
```


Lägger till en ny resurs på den angivna positionen i en projekts resurskollektion.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| resourceName | java.lang.String | Namn på en resurs. |
| beforeResourceId | int | Position för den föregående resursen i en projekts resurskollektion. |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### clear() {#clear--}
```
public final void clear()
```


Direkt rensning stöds inte, den här metoden kastar bara UnsupportedOperationException.

### contains(Object o) {#contains-java.lang.Object-}
```
public final boolean contains(Object o)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### get(int index) {#get-int-}
```
public Resource get(int index)
```


(@inheritDoc\}

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - \{@inheritDoc\}
### getById(int id) {#getById-int-}
```
public final Resource getById(int id)
```


Returnerar en resurs med det angivna id:t.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | id | int | Det angivna id:t. |

--------------------

O(1)-komplexitet. |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Resource with the specified id if present; otherwise, null.
### getByUid(int uid) {#getByUid-int-}
```
public final Resource getByUid(int uid)
```


Returnerar en resurs med den angivna Uid:n.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | uid | int | Det angivna uid. |

--------------------

O(1)-komplexitet. |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Resource with the specified uid if present; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Hämtar föräldraprojektet för ResourceCollection-objektet.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the ResourceCollection object.
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public final int indexOf(Object o)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
int – \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```




**Returns:**
boolean - \{@inheritDoc\}
### iterator() {#iterator--}
```
public final Iterator<Resource> iterator()
```


Returnerar en enumerator för denna samling.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Resource&gt; - en enumerator för denna samling.
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```


Detta är stub-implementationen av Collections remove‑metod, som bara kastar UnsupportedOperationException.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| o | java.lang.Object | objektet att ta bort. |

**Returns:**
boolean - `true` om objektet togs bort; `false` annars.
### size() {#size--}
```
public final int size()
```


Hämtar antalet element som finns i ResourceCollection.

--------------------

Skrivskyddad `int`.

**Returns:**
int - antalet element som finns i ResourceCollection.
### sort(Comparator&lt;? super Resource&gt; comparer) {#sort-java.util.Comparator---super-com.aspose.tasks.Resource--}
```
public final void sort(Comparator<? super Resource> comparer)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| jämförare | java.util.Comparator&lt;? super com.aspose.tasks.Resource&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<Resource> toList()
```


Konverterar ResourceCollection-objektet till en lista av [Resource](../../com.aspose.tasks/resource) objekt.

**Returns:**
java.util.List&lt;com.aspose.tasks.Resource&gt; - Lista över [Resource](../../com.aspose.tasks/resource) objekt.
