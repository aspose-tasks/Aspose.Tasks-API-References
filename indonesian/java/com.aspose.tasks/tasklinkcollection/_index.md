---
title: "TaskLinkCollection"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili koleksi objek."
type: docs
weight: 296
url: /id/java/com.aspose.tasks/tasklinkcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class TaskLinkCollection extends AbstractList<TaskLink>
```

Mewakili kumpulan [Task](../../com.aspose.tasks/task) objek.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [add(Task pred, Task succ)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-) | Mengembalikan sebuah instance Finish-Start [TaskLink](../../com.aspose.tasks/tasklink) yang telah ditambahkan ke objek TaskLinkCollection. |
| [add(Task pred, Task succ, int linkType)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-) | Mengembalikan sebuah instance [TaskLink](../../com.aspose.tasks/tasklink) yang telah ditambahkan ke objek TaskLinkCollection. |
| [add(Task pred, Task succ, int linkType, Duration lag)](#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-com.aspose.tasks.Duration-) | Mengembalikan sebuah instance [TaskLink](../../com.aspose.tasks/tasklink) yang telah ditambahkan ke objek TaskLinkCollection. |
| [add(TaskLink e)](#add-com.aspose.tasks.TaskLink-) | Ini adalah implementasi stub dari metode Add pada ICollection, yang hanya melempar UnsupportedOperationException |
| [clear()](#clear--) | Dicadangkan untuk penggunaan internal. |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getParentProject()](#getParentProject--) | Mendapatkan proyek induk dari objek ResourceAssignmentCollection. |
| [remove(int index)](#remove-int-) | Menghapus elemen pada posisi yang ditentukan dalam koleksi ini dan mengembalikan elemen yang dihapus dari koleksi. |
| [remove(Object item)](#remove-java.lang.Object-) | Menghapus tautan tugas dari sebuah proyek. |
| [size()](#size--) | Mengembalikan jumlah objek yang terdapat dalam objek `TaskLinkCollection` ini. |
| [sort(Comparator&lt;? super TaskLink&gt; c)](#sort-java.util.Comparator---super-com.aspose.tasks.TaskLink--) | \{@inheritDoc\} |
| [toList()](#toList--) | Mengonversi objek TaskLinkCollection menjadi daftar [TaskLink](../../com.aspose.tasks/tasklink) objek. |
### add(Task pred, Task succ) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-}
```
public final TaskLink add(Task pred, Task succ)
```


Mengembalikan sebuah instance Finish-Start [TaskLink](../../com.aspose.tasks/tasklink) yang telah ditambahkan ke objek TaskLinkCollection.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | Tugas pendahulu. |
| succ | [Task](../../com.aspose.tasks/task) | Tugas penerus. |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link instance which has been added to this object.
### add(Task pred, Task succ, int linkType) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-}
```
public final TaskLink add(Task pred, Task succ, int linkType)
```


Mengembalikan sebuah instance [TaskLink](../../com.aspose.tasks/tasklink) yang telah ditambahkan ke objek TaskLinkCollection.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | Tugas pendahulu. |
| succ | [Task](../../com.aspose.tasks/task) | Tugas penerus. |
| linkType | int | Tipe tautan [TaskLinkType](../../com.aspose.tasks/tasklinktype) |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link instance which has been added to this object.
### add(Task pred, Task succ, int linkType, Duration lag) {#add-com.aspose.tasks.Task-com.aspose.tasks.Task-int-com.aspose.tasks.Duration-}
```
public final TaskLink add(Task pred, Task succ, int linkType, Duration lag)
```


Mengembalikan sebuah instance [TaskLink](../../com.aspose.tasks/tasklink) yang telah ditambahkan ke objek TaskLinkCollection.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| pred | [Task](../../com.aspose.tasks/task) | Tugas pendahulu. |
| succ | [Task](../../com.aspose.tasks/task) | Tugas penerus. |
| linkType | int | Tipe tautan [TaskLinkType](../../com.aspose.tasks/tasklinktype) |
| lag | [Duration](../../com.aspose.tasks/duration) | Tunda tautan [Duration](../../com.aspose.tasks/duration). |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - a task link which has been added to this object.
### add(TaskLink e) {#add-com.aspose.tasks.TaskLink-}
```
public final boolean add(TaskLink e)
```


Ini adalah implementasi stub dari metode Add pada ICollection, yang hanya melempar UnsupportedOperationException

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| e | [TaskLink](../../com.aspose.tasks/tasklink) | Item yang akan ditambahkan. |

**Returns:**
boolean - \{@inheritDoc\}
### clear() {#clear--}
```
public final void clear()
```


Dicadangkan untuk penggunaan internal.

### get(int index) {#get-int-}
```
public TaskLink get(int index)
```


(@inheritDoc\}

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - \{@inheritDoc\}
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Mendapatkan proyek induk dari objek ResourceAssignmentCollection.

**Returns:**
[Project](../../com.aspose.tasks/project) - parent `Project` for this object.
### remove(int index) {#remove-int-}
```
public final TaskLink remove(int index)
```


Menghapus elemen pada posisi yang ditentukan dalam koleksi ini dan mengembalikan elemen yang dihapus dari koleksi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| index | int | posisi yang ditentukan untuk menghapus elemen pada. |

**Returns:**
[TaskLink](../../com.aspose.tasks/tasklink) - the element that was removed from the collection.
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


Menghapus tautan tugas dari sebuah proyek.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| item | java.lang.Object | instance yang ditentukan dari kelas `TaskLink` untuk dihapus. |

**Returns:**
boolean - mengembalikan instance kelas `TaskLink` yang telah dihapus dari koleksi ini.
### size() {#size--}
```
public final int size()
```


Mengembalikan jumlah objek yang terdapat dalam objek `TaskLinkCollection` ini. Hanya baca `int`.

**Returns:**
int - mengembalikan jumlah objek yang terdapat dalam koleksi ini.
### sort(Comparator&lt;? super TaskLink&gt; c) {#sort-java.util.Comparator---super-com.aspose.tasks.TaskLink--}
```
public void sort(Comparator<? super TaskLink> c)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| c | java.util.Comparator&lt;? super com.aspose.tasks.TaskLink&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<TaskLink> toList()
```


Mengonversi objek TaskLinkCollection menjadi daftar [TaskLink](../../com.aspose.tasks/tasklink) objek.

**Returns:**
java.util.List&lt;com.aspose.tasks.TaskLink&gt; - Daftar [TaskLink](../../com.aspose.tasks/tasklink) objek.
