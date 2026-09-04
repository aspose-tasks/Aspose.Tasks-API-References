---
title: "ResourceAssignmentCollection"
second_title: "Aspose.Tasks for Java API Reference"
description: "Stellt eine Sammlung von Objekten dar."
type: docs
weight: 250
url: /de/java/com.aspose.tasks/resourceassignmentcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class ResourceAssignmentCollection extends AbstractList<ResourceAssignment>
```

Stellt eine Sammlung von [ResourceAssignment](../../com.aspose.tasks/resourceassignment)-Objekten dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [add(ResourceAssignment item)](#add-com.aspose.tasks.ResourceAssignment-) | Dies ist die Stub‑Implementierung der Add‑Methode von ICollection, die nur UnsupportedOperationException wirft. |
| [add(Task task, Resource resource)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-) | Fügt der ResourceAssignmentCollection eine neue Zuordnung hinzu. |
| [add(Task task, Resource resource, double units)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-double-) | Fügt der ResourceAssignmentCollection eine neue Zuordnung hinzu. |
| [add(Task task, Resource resource, BigDecimal cost)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-java.math.BigDecimal-) | Fügt der ResourceAssignmentCollection eine neue Zuordnung hinzu. |
| [clear()](#clear--) | Entfernt alle Elemente aus der Sammlung. |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getByUid(int uid)](#getByUid-int-) | Gibt eine Zuordnung mit der angegebenen UID zurück. |
| [getParentProject()](#getParentProject--) | Ermittelt das übergeordnete Projekt des ResourceAssignmentCollection-Objekts. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Liefert einen Wert, der angibt, ob diese Sammlung schreibgeschützt ist. |
| [iterator()](#iterator--) | Gibt einen Enumerator für diese Sammlung zurück. |
| [remove(int index)](#remove-int-) | \{@inheritDoc\} |
| [remove(Object o)](#remove-java.lang.Object-) | Entfernt die angegebene Zuordnung aus der Sammlung, wenn sie nicht schreibgeschützt ist, andernfalls wird eine UnsupportedOperationException ausgelöst. |
| [size()](#size--) | Ermittelt die Anzahl der in der ResourceAssignmentCollection enthaltenen Objekte. |
| [toList()](#toList--) | Konvertiert das ResourceAssignmentCollection-Objekt in eine Liste von [ResourceAssignment](../../com.aspose.tasks/resourceassignment)-Objekten. |
### add(ResourceAssignment item) {#add-com.aspose.tasks.ResourceAssignment-}
```
public final boolean add(ResourceAssignment item)
```


Dies ist die Stub‑Implementierung der Add‑Methode von ICollection, die nur UnsupportedOperationException wirft.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| item | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | Das zu entfernende Element. |

**Returns:**
boolean - \\{@inheritDoc\\}
### add(Task task, Resource resource) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-}
```
public final ResourceAssignment add(Task task, Resource resource)
```


Fügt der ResourceAssignmentCollection eine neue Zuordnung hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Eine zuzuweisende Aufgabe. |
| resource | [Resource](../../com.aspose.tasks/resource) | Eine zuzuweisende Ressource. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### add(Task task, Resource resource, double units) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-double-}
```
public final ResourceAssignment add(Task task, Resource resource, double units)
```


Fügt der ResourceAssignmentCollection eine neue Zuordnung hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Eine zuzuweisende Aufgabe. |
| resource | [Resource](../../com.aspose.tasks/resource) | Eine zuzuweisende Ressource. |
| Einheiten | double | Die Anzahl der Einheiten für eine neue Zuordnung. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### add(Task task, Resource resource, BigDecimal cost) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-java.math.BigDecimal-}
```
public final ResourceAssignment add(Task task, Resource resource, BigDecimal cost)
```


Fügt der ResourceAssignmentCollection eine neue Zuordnung hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Eine zuzuweisende Aufgabe. |
| resource | [Resource](../../com.aspose.tasks/resource) | Eine Kostenressource, die zugewiesen werden soll. |
| Kosten | java.math.BigDecimal | Die Kosten für eine neue Zuordnung. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### clear() {#clear--}
```
public void clear()
```


Entfernt alle Elemente aus der Sammlung.

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
public ResourceAssignment get(int index)
```


(@inheritDoc\}

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | \{@inheritDoc\} |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - \{@inheritDoc\}
### getByUid(int uid) {#getByUid-int-}
```
public final ResourceAssignment getByUid(int uid)
```


Gibt eine Zuordnung mit der angegebenen UID zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | uid | int | Die angegebene UID. |

--------------------

O(1)-Komplexität. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - ResourceAssignment with the specified uid if present; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Ermittelt das übergeordnete Projekt des ResourceAssignmentCollection-Objekts.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the ResourceAssignmentCollection object.
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


Liefert einen Wert, der angibt, ob diese Sammlung schreibgeschützt ist.

**Returns:**
boolean - ein Wert, der angibt, ob diese Sammlung schreibgeschützt ist.
### iterator() {#iterator--}
```
public final Iterator<ResourceAssignment> iterator()
```


Gibt einen Enumerator für diese Sammlung zurück.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.ResourceAssignment&gt; - ein Enumerator für diese Sammlung.
### remove(int index) {#remove-int-}
```
public ResourceAssignment remove(int index)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | \{@inheritDoc\} |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - \{@inheritDoc\}
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```


Entfernt die angegebene Zuordnung aus der Sammlung, wenn sie nicht schreibgeschützt ist, andernfalls wird eine UnsupportedOperationException ausgelöst.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| o | java.lang.Object | Die zu entfernende Zuordnung. |

**Returns:**
boolean - true, wenn das angegebene Element entfernt wurde, sonst false.
### size() {#size--}
```
public final int size()
```


Ermittelt die Anzahl der in der ResourceAssignmentCollection enthaltenen Objekte.

**Returns:**
int - die Anzahl der in der ResourceAssignmentCollection enthaltenen Objekte.
### toList() {#toList--}
```
public final List<ResourceAssignment> toList()
```


Konvertiert das ResourceAssignmentCollection-Objekt in eine Liste von [ResourceAssignment](../../com.aspose.tasks/resourceassignment)-Objekten.

**Returns:**
java.util.List&lt;com.aspose.tasks.ResourceAssignment&gt; - Liste von [ResourceAssignment](../../com.aspose.tasks/resourceassignment)-Objekten.
