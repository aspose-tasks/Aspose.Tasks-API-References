---
title: "ResourceAssignmentCollection"
second_title: "Aspose.Tasks for Java API-referentie"
description: "Stelt een collectie van objecten voor."
type: docs
weight: 250
url: /nl/java/com.aspose.tasks/resourceassignmentcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class ResourceAssignmentCollection extends AbstractList<ResourceAssignment>
```

Stelt een collectie van [ResourceAssignment](../../com.aspose.tasks/resourceassignment) objecten voor.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [add(ResourceAssignment item)](#add-com.aspose.tasks.ResourceAssignment-) | Dit is de stub‑implementatie van de Add‑methode van ICollection, die alleen UnsupportedOperationException gooit. |
| [add(Task task, Resource resource)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-) | Voegt een nieuwe toewijzing toe aan de ResourceAssignmentCollection. |
| [add(Task task, Resource resource, double units)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-double-) | Voegt een nieuwe toewijzing toe aan de ResourceAssignmentCollection. |
| [add(Task task, Resource resource, BigDecimal cost)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-java.math.BigDecimal-) | Voegt een nieuwe toewijzing toe aan de ResourceAssignmentCollection. |
| [clear()](#clear--) | Verwijdert alle items uit de collectie. |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | (@inheritDoc\\} |
| [getByUid(int uid)](#getByUid-int-) | Retourneert een toewijzing met de opgegeven uid. |
| [getParentProject()](#getParentProject--) | Haalt het bovenliggende project op van het ResourceAssignmentCollection-object. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Haalt een waarde op die aangeeft of deze collectie alleen-lezen is. |
| [iterator()](#iterator--) | Retourneert een enumerator voor deze collectie. |
| [remove(int index)](#remove-int-) | \{@inheritDoc\} |
| [remove(Object o)](#remove-java.lang.Object-) | Verwijdert de opgegeven toewijzing uit de collectie, als deze niet alleen-lezen is, anders wordt UnsupportedOperationException gegooid. |
| [size()](#size--) | Haalt het aantal objecten op dat in de ResourceAssignmentCollection zit. |
| [toList()](#toList--) | Converteert het ResourceAssignmentCollection-object naar een lijst van [ResourceAssignment](../../com.aspose.tasks/resourceassignment) objecten. |
### add(ResourceAssignment item) {#add-com.aspose.tasks.ResourceAssignment-}
```
public final boolean add(ResourceAssignment item)
```


Dit is de stub‑implementatie van de Add‑methode van ICollection, die alleen UnsupportedOperationException gooit.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| item | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | Het item om te verwijderen. |

**Returns:**
boolean - \{@inheritDoc\}
### add(Task task, Resource resource) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-}
```
public final ResourceAssignment add(Task task, Resource resource)
```


Voegt een nieuwe toewijzing toe aan de ResourceAssignmentCollection.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Een taak die moet worden toegewezen. |
| resource | [Resource](../../com.aspose.tasks/resource) | Een resource die moet worden toegewezen. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### add(Task task, Resource resource, double units) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-double-}
```
public final ResourceAssignment add(Task task, Resource resource, double units)
```


Voegt een nieuwe toewijzing toe aan de ResourceAssignmentCollection.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Een taak die moet worden toegewezen. |
| resource | [Resource](../../com.aspose.tasks/resource) | Een resource die moet worden toegewezen. |
| eenheden | double | Het aantal eenheden voor een nieuwe toewijzing. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### add(Task task, Resource resource, BigDecimal cost) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-java.math.BigDecimal-}
```
public final ResourceAssignment add(Task task, Resource resource, BigDecimal cost)
```


Voegt een nieuwe toewijzing toe aan de ResourceAssignmentCollection.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Een taak die moet worden toegewezen. |
| resource | [Resource](../../com.aspose.tasks/resource) | Een kostresource die moet worden toegewezen. |
| kosten | java.math.BigDecimal | De kosten voor een nieuwe toewijzing. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### clear() {#clear--}
```
public void clear()
```


Verwijdert alle items uit de collectie.

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
public ResourceAssignment get(int index)
```


(@inheritDoc\\}

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - \{@inheritDoc\}
### getByUid(int uid) {#getByUid-int-}
```
public final ResourceAssignment getByUid(int uid)
```


Retourneert een toewijzing met de opgegeven uid.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | uid | int | De opgegeven uid. |

--------------------

O(1)-complexiteit. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - ResourceAssignment with the specified uid if present; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Haalt het bovenliggende project op van het ResourceAssignmentCollection-object.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the ResourceAssignmentCollection object.
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


Haalt een waarde op die aangeeft of deze collectie alleen-lezen is.

**Returns:**
boolean - een waarde die aangeeft of deze collectie alleen-lezen is.
### iterator() {#iterator--}
```
public final Iterator<ResourceAssignment> iterator()
```


Retourneert een enumerator voor deze collectie.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.ResourceAssignment&gt; - een enumerator voor deze collectie.
### remove(int index) {#remove-int-}
```
public ResourceAssignment remove(int index)
```




**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - \{@inheritDoc\}
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```


Verwijdert de opgegeven toewijzing uit de collectie, als deze niet alleen-lezen is, anders wordt UnsupportedOperationException gegooid.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| o | java.lang.Object | De toewijzing om te verwijderen. |

**Returns:**
boolean - true, als het opgegeven item is verwijderd, anders false.
### size() {#size--}
```
public final int size()
```


Haalt het aantal objecten op dat in de ResourceAssignmentCollection zit.

**Returns:**
int - het aantal objecten dat zich in de ResourceAssignmentCollection bevindt.
### toList() {#toList--}
```
public final List<ResourceAssignment> toList()
```


Converteert het ResourceAssignmentCollection-object naar een lijst van [ResourceAssignment](../../com.aspose.tasks/resourceassignment) objecten.

**Returns:**
java.util.List&lt;com.aspose.tasks.ResourceAssignment&gt; - Lijst van [ResourceAssignment](../../com.aspose.tasks/resourceassignment) objecten.
