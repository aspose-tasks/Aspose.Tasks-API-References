---
title: "ResourceCollection"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een collectie van objecten voor."
type: docs
weight: 251
url: /nl/java/com.aspose.tasks/resourcecollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class ResourceCollection extends AbstractList<Resource>
```

Stelt een verzameling van [Resource](../../com.aspose.tasks/resource) objecten voor.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [add()](#add--) | Voegt een nieuwe resource toe op de laatste positie van een projectresourceverzameling. |
| [add(Resource e)](#add-com.aspose.tasks.Resource-) | \{@inheritDoc\} |
| [add(String resourceName)](#add-java.lang.String-) | Voegt een nieuwe resource toe op de laatste positie van een projectresourceverzameling. |
| [add(String resourceName, int beforeResourceId)](#add-java.lang.String-int-) | Voegt een nieuwe resource toe op de opgegeven positie van een projectresourcesverzameling. |
| [clear()](#clear--) | Direct wissen wordt niet ondersteund, deze methode gooit alleen UnsupportedOperationException. |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | (@inheritDoc\\} |
| [getById(int id)](#getById-int-) | Retourneert een resource met de opgegeven id. |
| [getByUid(int uid)](#getByUid-int-) | Retourneert een resource met de opgegeven Uid. |
| [getParentProject()](#getParentProject--) | Haalt het bovenliggende project op van het ResourceCollection-object. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | \{@inheritDoc\} |
| [iterator()](#iterator--) | Retourneert een enumerator voor deze collectie. |
| [remove(Object o)](#remove-java.lang.Object-) | Dit is de stub-implementatie van de remove-methode van Collection, die alleen UnsupportedOperationException gooit. |
| [size()](#size--) | Haalt het aantal elementen op dat in de ResourceCollection zit. |
| [sort(Comparator&lt;? super Resource&gt; comparer)](#sort-java.util.Comparator---super-com.aspose.tasks.Resource--) | \{@inheritDoc\} |
| [toList()](#toList--) | Converteert het ResourceCollection-object naar een lijst van [Resource](../../com.aspose.tasks/resource) objecten. |
### add() {#add--}
```
public final Resource add()
```


Voegt een nieuwe resource toe op de laatste positie van een projectresourceverzameling.

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### add(Resource e) {#add-com.aspose.tasks.Resource-}
```
public final boolean add(Resource e)
```




**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| e | [Resource](../../com.aspose.tasks/resource) | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### add(String resourceName) {#add-java.lang.String-}
```
public final Resource add(String resourceName)
```


Voegt een nieuwe resource toe op de laatste positie van een projectresourceverzameling.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| resourceName | java.lang.String | Naam van een resource. |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### add(String resourceName, int beforeResourceId) {#add-java.lang.String-int-}
```
public final Resource add(String resourceName, int beforeResourceId)
```


Voegt een nieuwe resource toe op de opgegeven positie van een projectresourcesverzameling.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| resourceName | java.lang.String | Naam van een resource. |
| beforeResourceId | int | Positie van de vorige resource in een projectresourcesverzameling. |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### clear() {#clear--}
```
public final void clear()
```


Direct wissen wordt niet ondersteund, deze methode gooit alleen UnsupportedOperationException.

### contains(Object o) {#contains-java.lang.Object-}
```
public final boolean contains(Object o)
```




**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### get(int index) {#get-int-}
```
public Resource get(int index)
```


(@inheritDoc\\}

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - \{@inheritDoc\}
### getById(int id) {#getById-int-}
```
public final Resource getById(int id)
```


Retourneert een resource met de opgegeven id.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | id | int | De opgegeven id. |

--------------------

O(1)-complexiteit. |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Resource with the specified id if present; otherwise, null.
### getByUid(int uid) {#getByUid-int-}
```
public final Resource getByUid(int uid)
```


Retourneert een resource met de opgegeven Uid.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | uid | int | De opgegeven uid. |

--------------------

O(1)-complexiteit. |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Resource with the specified uid if present; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Haalt het bovenliggende project op van het ResourceCollection-object.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the ResourceCollection object.
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public final int indexOf(Object o)
```




**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
int - \{@inheritDoc\}
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


Retourneert een enumerator voor deze collectie.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Resource&gt; - een enumerator voor deze verzameling.
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```


Dit is de stub-implementatie van de remove-methode van Collection, die alleen UnsupportedOperationException gooit.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| o | java.lang.Object | het te verwijderen item. |

**Returns:**
boolean - `true` als het item is verwijderd; `false` anders.
### size() {#size--}
```
public final int size()
```


Haalt het aantal elementen op dat in de ResourceCollection zit.

--------------------

Alleen-lezen `int`.

**Returns:**
int - het aantal elementen dat in de ResourceCollection zit.
### sort(Comparator&lt;? super Resource&gt; comparer) {#sort-java.util.Comparator---super-com.aspose.tasks.Resource--}
```
public final void sort(Comparator<? super Resource> comparer)
```




**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| vergelijker | java.util.Comparator&lt;? super com.aspose.tasks.Resource&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<Resource> toList()
```


Converteert het ResourceCollection-object naar een lijst van [Resource](../../com.aspose.tasks/resource) objecten.

**Returns:**
java.util.List&lt;com.aspose.tasks.Resource&gt; - Lijst van [Resource](../../com.aspose.tasks/resource) objecten.
