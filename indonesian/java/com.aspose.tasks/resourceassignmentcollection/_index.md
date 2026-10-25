---
title: "ResourceAssignmentCollection"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili koleksi objek."
type: docs
weight: 250
url: /id/java/com.aspose.tasks/resourceassignmentcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class ResourceAssignmentCollection extends AbstractList<ResourceAssignment>
```

Mewakili koleksi objek [ResourceAssignment](../../com.aspose.tasks/resourceassignment).
## Metode

| Metode | Deskripsi |
| --- | --- |
| [add(ResourceAssignment item)](#add-com.aspose.tasks.ResourceAssignment-) | Ini adalah implementasi stub dari metode Add pada ICollection, yang hanya melempar UnsupportedOperationException |
| [add(Task task, Resource resource)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-) | Menambahkan penugasan baru ke ResourceAssignmentCollection. |
| [add(Task task, Resource resource, double units)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-double-) | Menambahkan penugasan baru ke ResourceAssignmentCollection. |
| [add(Task task, Resource resource, BigDecimal cost)](#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-java.math.BigDecimal-) | Menambahkan penugasan baru ke ResourceAssignmentCollection. |
| [clear()](#clear--) | Menghapus semua item dari koleksi. |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getByUid(int uid)](#getByUid-int-) | Mengembalikan penugasan dengan uid yang ditentukan. |
| [getParentProject()](#getParentProject--) | Mendapatkan proyek induk dari objek ResourceAssignmentCollection. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Mendapatkan nilai yang menunjukkan apakah koleksi ini hanya-baca. |
| [iterator()](#iterator--) | Mengembalikan enumerator untuk koleksi ini. |
| [remove(int index)](#remove-int-) | \{@inheritDoc\} |
| [remove(Object o)](#remove-java.lang.Object-) | Menghapus penugasan yang ditentukan dari koleksi, jika tidak bersifat read-only, jika tidak akan melempar UnsupportedOperationException. |
| [size()](#size--) | Mendapatkan jumlah objek yang terdapat dalam ResourceAssignmentCollection. |
| [toList()](#toList--) | Mengonversi objek ResourceAssignmentCollection menjadi daftar objek [ResourceAssignment](../../com.aspose.tasks/resourceassignment). |
### add(ResourceAssignment item) {#add-com.aspose.tasks.ResourceAssignment-}
```
public final boolean add(ResourceAssignment item)
```


Ini adalah implementasi stub dari metode Add pada ICollection, yang hanya melempar UnsupportedOperationException

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| item | [ResourceAssignment](../../com.aspose.tasks/resourceassignment) | Item yang akan dihapus. |

**Returns:**
boolean - \{@inheritDoc\}
### add(Task task, Resource resource) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-}
```
public final ResourceAssignment add(Task task, Resource resource)
```


Menambahkan penugasan baru ke ResourceAssignmentCollection.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Sebuah tugas yang akan ditugaskan. |
| resource | [Resource](../../com.aspose.tasks/resource) | Sebuah sumber daya yang akan ditugaskan. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### add(Task task, Resource resource, double units) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-double-}
```
public final ResourceAssignment add(Task task, Resource resource, double units)
```


Menambahkan penugasan baru ke ResourceAssignmentCollection.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Sebuah tugas yang akan ditugaskan. |
| resource | [Resource](../../com.aspose.tasks/resource) | Sebuah sumber daya yang akan ditugaskan. |
| unit | double | Jumlah unit untuk penugasan baru. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### add(Task task, Resource resource, BigDecimal cost) {#add-com.aspose.tasks.Task-com.aspose.tasks.Resource-java.math.BigDecimal-}
```
public final ResourceAssignment add(Task task, Resource resource, BigDecimal cost)
```


Menambahkan penugasan baru ke ResourceAssignmentCollection.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Sebuah tugas yang akan ditugaskan. |
| resource | [Resource](../../com.aspose.tasks/resource) | Sebuah sumber daya biaya yang akan ditugaskan. |
| biaya | java.math.BigDecimal | Biaya untuk penugasan baru. |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - Added assignment.
### clear() {#clear--}
```
public void clear()
```


Menghapus semua item dari koleksi.

### contains(Object o) {#contains-java.lang.Object-}
```
public final boolean contains(Object o)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
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
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - \{@inheritDoc\}
### getByUid(int uid) {#getByUid-int-}
```
public final ResourceAssignment getByUid(int uid)
```


Mengembalikan penugasan dengan uid yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | uid | int | Uid yang ditentukan. |

--------------------

Kompleksitas O(1). |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - ResourceAssignment with the specified uid if present; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Mendapatkan proyek induk dari objek ResourceAssignmentCollection.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the ResourceAssignmentCollection object.
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public final int indexOf(Object o)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| o | java.lang.Object | \{@inheritDoc\} |

**Returns:**
int - \{@inheritDoc\}
### isReadOnly() {#isReadOnly--}
```
public final boolean isReadOnly()
```


Mendapatkan nilai yang menunjukkan apakah koleksi ini hanya-baca.

**Returns:**
boolean - nilai yang menunjukkan apakah koleksi ini hanya-baca.
### iterator() {#iterator--}
```
public final Iterator<ResourceAssignment> iterator()
```


Mengembalikan enumerator untuk koleksi ini.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.ResourceAssignment&gt; - sebuah enumerator untuk koleksi ini.
### remove(int index) {#remove-int-}
```
public ResourceAssignment remove(int index)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[ResourceAssignment](../../com.aspose.tasks/resourceassignment) - \{@inheritDoc\}
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```


Menghapus penugasan yang ditentukan dari koleksi, jika tidak bersifat read-only, jika tidak akan melempar UnsupportedOperationException.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| o | java.lang.Object | Penugasan untuk dihapus. |

**Returns:**
boolean - true, jika item yang ditentukan dihapus, false jika tidak.
### size() {#size--}
```
public final int size()
```


Mendapatkan jumlah objek yang terdapat dalam ResourceAssignmentCollection.

**Returns:**
int - jumlah objek yang terdapat dalam ResourceAssignmentCollection.
### toList() {#toList--}
```
public final List<ResourceAssignment> toList()
```


Mengonversi objek ResourceAssignmentCollection menjadi daftar objek [ResourceAssignment](../../com.aspose.tasks/resourceassignment).

**Returns:**
java.util.List&lt;com.aspose.tasks.ResourceAssignment&gt; - Daftar objek [ResourceAssignment](../../com.aspose.tasks/resourceassignment).
