---
title: "ResourceCollection"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili koleksi objek."
type: docs
weight: 251
url: /id/java/com.aspose.tasks/resourcecollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class ResourceCollection extends AbstractList<Resource>
```

Mewakili kumpulan objek [Resource](../../com.aspose.tasks/resource).
## Metode

| Metode | Deskripsi |
| --- | --- |
| [add()](#add--) | Menambahkan sumber baru pada posisi terakhir dalam koleksi sumber daya proyek. |
| [add(Resource e)](#add-com.aspose.tasks.Resource-) | \{@inheritDoc\} |
| [add(String resourceName)](#add-java.lang.String-) | Menambahkan sumber baru pada posisi terakhir dalam koleksi sumber daya proyek. |
| [add(String resourceName, int beforeResourceId)](#add-java.lang.String-int-) | Menambahkan sumber daya baru pada posisi yang ditentukan dalam koleksi sumber daya proyek. |
| [clear()](#clear--) | Penghapusan langsung tidak didukung, metode ini hanya melempar UnsupportedOperationException. |
| [contains(Object o)](#contains-java.lang.Object-) | \{@inheritDoc\} |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getById(int id)](#getById-int-) | Mengembalikan sumber daya dengan id yang ditentukan. |
| [getByUid(int uid)](#getByUid-int-) | Mengembalikan sumber daya dengan Uid yang ditentukan. |
| [getParentProject()](#getParentProject--) | Mendapatkan proyek induk dari objek ResourceCollection. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | \{@inheritDoc\} |
| [iterator()](#iterator--) | Mengembalikan enumerator untuk koleksi ini. |
| [remove(Object o)](#remove-java.lang.Object-) | Ini adalah implementasi stub dari metode remove pada Collection, yang hanya melempar UnsupportedOperationException |
| [size()](#size--) | Mendapatkan jumlah elemen yang terdapat dalam ResourceCollection. |
| [sort(Comparator&lt;? super Resource&gt; comparer)](#sort-java.util.Comparator---super-com.aspose.tasks.Resource--) | \{@inheritDoc\} |
| [toList()](#toList--) | Mengonversi objek ResourceCollection menjadi daftar [Resource](../../com.aspose.tasks/resource) objek. |
### add() {#add--}
```
public final Resource add()
```


Menambahkan sumber baru pada posisi terakhir dalam koleksi sumber daya proyek.

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### add(Resource e) {#add-com.aspose.tasks.Resource-}
```
public final boolean add(Resource e)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| e | [Resource](../../com.aspose.tasks/resource) | \{@inheritDoc\} |

**Returns:**
boolean - \{@inheritDoc\}
### add(String resourceName) {#add-java.lang.String-}
```
public final Resource add(String resourceName)
```


Menambahkan sumber baru pada posisi terakhir dalam koleksi sumber daya proyek.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| resourceName | java.lang.String | Nama sebuah sumber daya. |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### add(String resourceName, int beforeResourceId) {#add-java.lang.String-int-}
```
public final Resource add(String resourceName, int beforeResourceId)
```


Menambahkan sumber daya baru pada posisi yang ditentukan dalam koleksi sumber daya proyek.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| resourceName | java.lang.String | Nama sebuah sumber daya. |
| beforeResourceId | int | Posisi sumber daya sebelumnya dalam koleksi sumber daya proyek. |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Added resource.
### clear() {#clear--}
```
public final void clear()
```


Penghapusan langsung tidak didukung, metode ini hanya melempar UnsupportedOperationException.

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
public Resource get(int index)
```


(@inheritDoc\}

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - \{@inheritDoc\}
### getById(int id) {#getById-int-}
```
public final Resource getById(int id)
```


Mengembalikan sumber daya dengan id yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | id | int | Id yang ditentukan. |

--------------------

Kompleksitas O(1). |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Resource with the specified id if present; otherwise, null.
### getByUid(int uid) {#getByUid-int-}
```
public final Resource getByUid(int uid)
```


Mengembalikan sumber daya dengan Uid yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | uid | int | Uid yang ditentukan. |

--------------------

Kompleksitas O(1). |

**Returns:**
[Resource](../../com.aspose.tasks/resource) - Resource with the specified uid if present; otherwise, null.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Mendapatkan proyek induk dari objek ResourceCollection.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the ResourceCollection object.
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




**Returns:**
boolean - \{@inheritDoc\}
### iterator() {#iterator--}
```
public final Iterator<Resource> iterator()
```


Mengembalikan enumerator untuk koleksi ini.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Resource&gt; - enumerator untuk koleksi ini.
### remove(Object o) {#remove-java.lang.Object-}
```
public final boolean remove(Object o)
```


Ini adalah implementasi stub dari metode remove pada Collection, yang hanya melempar UnsupportedOperationException

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| o | java.lang.Object | item yang akan dihapus. |

**Returns:**
boolean - `true` jika item dihapus; `false` jika tidak.
### size() {#size--}
```
public final int size()
```


Mendapatkan jumlah elemen yang terdapat dalam ResourceCollection.

--------------------

Hanya-baca `int`.

**Returns:**
int - jumlah elemen yang terdapat dalam ResourceCollection.
### sort(Comparator&lt;? super Resource&gt; comparer) {#sort-java.util.Comparator---super-com.aspose.tasks.Resource--}
```
public final void sort(Comparator<? super Resource> comparer)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| comparer | java.util.Comparator&lt;? super com.aspose.tasks.Resource&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<Resource> toList()
```


Mengonversi objek ResourceCollection menjadi daftar [Resource](../../com.aspose.tasks/resource) objek.

**Returns:**
java.util.List&lt;com.aspose.tasks.Resource&gt; - Daftar [Resource](../../com.aspose.tasks/resource) objek.
