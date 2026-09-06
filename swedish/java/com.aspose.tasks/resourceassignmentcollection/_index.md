---
title: "ResourceAssignmentCollection"
second_title: "Aspose.Tasks for Java API-referens"
description: "Representerar en samling av  objekt."
type: docs
weight: 250
url: /sv/java/com.aspose.tasks/resourceassignmentcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class ResourceAssignmentCollection extends AbstractList<ResourceAssignment>
```

Representerar en samling av [ResourceAssignment](../../com.aspose.tasks/resourceassignment)-objekt.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(ResourceAssignment item)](#add-com.aspose.tasks.ResourceAssignment-) | Detta är stub-implementationen av ICollection:s Add‑metod, som endast kastar UnsupportedOperationException. |
| [add(Task task, Resource resource)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-) | Lägger till en ny tilldelning i ResourceAssignmentCollection. |
| [add(Task task, Resource resource, double units)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-double-) | Lägger till en ny tilldelning i ResourceAssignmentCollection. |
| [add(Task task, Resource resource, BigDecimal cost)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-java.math.BigDecimal-) | Lägger till en ny tilldelning i ResourceAssignmentCollection. |
| [clear()](#clear--) | Tar bort alla objekt från samlingen. |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getByUid(int uid)](#getByUid-int-) | Returnerar en tilldelning med det angivna uid‑värdet. |
| [getParentProject()](#getParentProject--) | Hämtar föräldraprojektet för ResourceAssignmentCollection-objektet. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Hämtar ett värde som indikerar om denna samling är skrivskyddad. |
| [iterator()](#iterator--) | Returnerar en enumerator för denna samling. |
| [remove(int index)](#remove-int-) | \{@inheritDoc\} |
| [remove(Object o)](#remove-java.lang.Object-) | Tar bort den angivna tilldelningen från samlingen, om den inte är skrivskyddad, annars kastas UnsupportedOperationException. |
| [size()](#size--) | Hämtar antalet objekt som finns i ResourceAssignmentCollection. |
| [toList()](#toList--) | Konverterar ResourceAssignmentCollection‑objektet till en lista av [ResourceAssignment](../../com.aspose.tasks/resourceassignment)-objekt. |
### add(ResourceAssignment item) {#add-com.aspose.tasks.ResourceAssignment-}
```
public final boolean add(ResourceAssignment item)
```


Detta är stub-implementationen av ICollection:s Add‑metod, som endast kastar UnsupportedOperationException.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| item | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | Objektet som ska tas bort. |

**Returns:**
boolean - \{@inheritDoc\}
### add(Task task, Resource resource) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-}
```
public final ResourceAssignment add(Task task, Resource resource)
```


Lägger till en ny tilldelning i ResourceAssignmentCollection.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | En uppgift att tilldela. |
| resource | [Resource](../../com.aspose.tasks/resource) | En resurs att tilldela. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### add(Task task, Resource resource, double units) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-double-}
```
public final ResourceAssignment add(Task task, Resource resource, double units)
```


Lägger till en ny tilldelning i ResourceAssignmentCollection.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | En uppgift att tilldela. |
| resource | [Resource](../../com.aspose.tasks/resource) | En resurs att tilldela. |
| enheter | double | Antalet enheter för en ny tilldelning. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### add(Task task, Resource resource, BigDecimal cost) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-java.math.BigDecimal-}
```
public final ResourceAssignment add(Task task, Resource resource, BigDecimal cost)
```


Lägger till en ny tilldelning i ResourceAssignmentCollection.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | En uppgift att tilldela. |
| resource | [Resource](../../com.aspose.tasks/resource) | En kostnadsresurs att tilldela. |
| kostnad | java.math.BigDecimal | Kostnaden för en ny tilldelning. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### clear() {#clear--}
```
public void clear()
```


Tar bort alla objekt från samlingen.

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
public ResourceAssignment get(int index)
```


(@inheritDoc\}

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - \{@inheritDoc\}
### getByUid(int uid) {#getByUid-int-}
```
public final ResourceAssignment getByUid(int uid)
```


Returnerar en tilldelning med det angivna uid‑värdet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | uid | int | Det angivna uid. |

--------------------

O(1)-komplexitet. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - ResourceAssignment with the specified uid if present; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Hämtar föräldraprojektet för ResourceAssignmentCollection-objektet.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the ResourceAssignmentCollection object.
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


Hämtar ett värde som indikerar om denna samling är skrivskyddad.

**Returns:**
boolean - ett värde som indikerar om denna samling är skrivskyddad.
### iterator() {#iterator--}
```
public final Iterator<ResourceAssignment> iterator()
```


Returnerar en enumerator för denna samling.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.ResourceAssignment&gt; - en enumerator för denna samling.
### remove(int index) {#remove-int-}
```
public ResourceAssignment remove(int index)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - \{@inheritDoc\}
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```


Tar bort den angivna tilldelningen från samlingen, om den inte är skrivskyddad, annars kastas UnsupportedOperationException.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| o | java.lang.Object | Tilldelningen att ta bort. |

**Returns:**
boolean - true, om angivet objekt togs bort, false annars.
### size() {#size--}
```
public final int size()
```


Hämtar antalet objekt som finns i ResourceAssignmentCollection.

**Returns:**
int - antalet objekt som finns i ResourceAssignmentCollection.
### toList() {#toList--}
```
public final List<ResourceAssignment> toList()
```


Konverterar ResourceAssignmentCollection‑objektet till en lista av [ResourceAssignment](../../com.aspose.tasks/resourceassignment)-objekt.

**Returns:**
java.util.List&lt;com.aspose.tasks.ResourceAssignment&gt; - Lista över [ResourceAssignment](../../com.aspose.tasks/resourceassignment)-objekt.
