---
title: "TaskCollection"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili koleksi objek."
type: docs
weight: 293
url: /id/java/com.aspose.tasks/taskcollection/
---

**Inheritance:**
java.lang.Object, java.util.AbstractCollection, java.util.AbstractList, com.aspose.tasks.AbstractList
```
public class TaskCollection extends AbstractList<Task>
```

Mewakili kumpulan [Task](../../com.aspose.tasks/task) objek.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [add()](#add--) | Menambahkan tugas baru ke koleksi tugas proyek pada tingkat outline yang sama dengan tugas terakhir. |
| [add(RecurringTaskParameters parameters)](#add-com.aspose.tasks.RecurringTaskParameters-) | Menyisipkan tugas baru sebelum tugas dengan id yang ditentukan dan pada tingkat outline yang sama. |
| [add(Task item)](#add-com.aspose.tasks.Task-) | Menambahkan tugas yang ditentukan ke instance dari kelas [TaskCollection](../../com.aspose.tasks/taskcollection). |
| [add(String taskName)](#add-java.lang.String-) | Menambahkan tugas baru ke koleksi tugas anak. |
| [add(String taskName, int beforeTaskId)](#add-java.lang.String-int-) | Menambahkan tugas berulang baru ke koleksi tugas anak. |
| [clear()](#clear--) | \{@inheritDoc\} |
| [contains(Task item)](#contains-com.aspose.tasks.Task-) | Memeriksa apakah koleksi berisi item yang ditentukan. |
| [get(int index)](#get-int-) | (@inheritDoc\} |
| [getById(int id)](#getById-int-) | Mengembalikan tugas dengan Id yang ditentukan yang nenek moyangnya adalah tugas induk dari koleksi ini. |
| [getByUid(int uid)](#getByUid-int-) | Mengembalikan tugas dengan Uid yang ditentukan yang nenek moyangnya adalah tugas induk dari koleksi ini. |
| [getParentProject()](#getParentProject--) | Mendapatkan proyek induk dari objek TaskCollection. |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | \{@inheritDoc\} |
| [isReadOnly()](#isReadOnly--) | Mendapatkan nilai yang menunjukkan apakah koleksi ini hanya-baca. |
| [iterator()](#iterator--) | Mengembalikan enumerator untuk koleksi ini. |
| [remove(Object item)](#remove-java.lang.Object-) | Ini adalah implementasi stub dari metode Remove pada ICollection, yang hanya melempar UnsupportedOperationException. |
| [size()](#size--) | Mendapatkan jumlah objek yang terkandung dalam TaskCollection. |
| [sort(Comparator&lt;? super Task&gt; c)](#sort-java.util.Comparator---super-com.aspose.tasks.Task--) | \{@inheritDoc\} |
| [toList()](#toList--) | Mengonversi objek TaskCollection menjadi daftar objek [Task](../../com.aspose.tasks/task). |
### add() {#add--}
```
public final Task add()
```


Menambahkan tugas baru ke koleksi tugas proyek pada tingkat outline yang sama dengan tugas terakhir.

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(RecurringTaskParameters parameters) {#add-com.aspose.tasks.RecurringTaskParameters-}
```
public final Task add(RecurringTaskParameters parameters)
```


Menyisipkan tugas baru sebelum tugas dengan id yang ditentukan dan pada tingkat outline yang sama.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| parameters | [RecurringTaskParameters](../../com.aspose.tasks/recurringtaskparameters) | Parameter yang ditentukan untuk pembuatan tugas berulang. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(Task item) {#add-com.aspose.tasks.Task-}
```
public final boolean add(Task item)
```


Tambahkan tugas yang ditentukan ke instance kelas [TaskCollection](../../com.aspose.tasks/taskcollection). Jika ParentProject.CalculationMode adalah None, pengguna harus memanggil Project.Recalculate() setelah menggunakan metode ini (Ini akan menjadwalkan ulang semua tugas proyek (tanggal mulai/selesai, mengatur tanggal awal/akhir) dan menghitung bidang yang bergantung seperti slack, bidang kerja dan biaya, id, serta tingkat outline). Jika ParentProject.CalculationMode adalah Manual, metode ini akan menghitung hanya id tugas, tingkat outline, dan nomor outline secara otomatis. Jika ParentProject.CalculationMode adalah Automatic, metode ini menjadwalkan ulang semua tugas proyek secara otomatis (tanggal mulai/selesai, mengatur tanggal awal/akhir, menghitung slack, bidang kerja dan biaya, menghitung ulang id dan tingkat outline).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| item | [Task](../../com.aspose.tasks/task) | tugas yang ditentukan yang harus ditambahkan ke koleksi tugas ini. |

**Returns:**
boolean - true jika operasi berhasil.
### add(String taskName) {#add-java.lang.String-}
```
public final Task add(String taskName)
```


Menambahkan tugas baru ke koleksi tugas anak.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| taskName | java.lang.String | nama tugas yang ditentukan. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the newly added instance of the [Task](../../com.aspose.tasks/task) class.
### add(String taskName, int beforeTaskId) {#add-java.lang.String-int-}
```
public final Task add(String taskName, int beforeTaskId)
```


Menambahkan tugas berulang baru ke koleksi tugas anak.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| taskName | java.lang.String | nama tugas yang ditentukan. |
| beforeTaskId | int | ID yang ditentukan dari tugas sebelum mana tugas baru akan disisipkan. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns a task which was inserted before a task with the specified id.
### clear() {#clear--}
```
public final void clear()
```




### contains(Task item) {#contains-com.aspose.tasks.Task-}
```
public final boolean contains(Task item)
```


Memeriksa apakah koleksi berisi item yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| item | [Task](../../com.aspose.tasks/task) | Item yang akan diperiksa. |

**Returns:**
boolean - true, jika koleksi berisi sebuah item, false jika tidak.
### get(int index) {#get-int-}
```
public Task get(int index)
```


(@inheritDoc\}

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| index | int | \{@inheritDoc\} |

**Returns:**
[Task](../../com.aspose.tasks/task) - \{@inheritDoc\}
### getById(int id) {#getById-int-}
```
public final Task getById(int id)
```


Mengembalikan tugas dengan Id yang ditentukan yang nenek moyangnya adalah tugas induk dari koleksi ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| id | int | TaskEntity Id |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the instance of [Task](../../com.aspose.tasks/task) class with the specified id whose ancestor is parent task of this collection.
### getByUid(int uid) {#getByUid-int-}
```
public final Task getByUid(int uid)
```


Mengembalikan tugas dengan Uid yang ditentukan yang nenek moyangnya adalah tugas induk dari koleksi ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| uid | int | TaskEntity Uid. |

**Returns:**
[Task](../../com.aspose.tasks/task) - returns the instance of [Task](../../com.aspose.tasks/task) class with the specified uid whose ancestor is parent task of this collection.
### getParentProject() {#getParentProject--}
```
public final Project getParentProject()
```


Mendapatkan proyek induk dari objek TaskCollection.

**Returns:**
[Project](../../com.aspose.tasks/project) - the parent project of the TaskCollection object.
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
public final Iterator<Task> iterator()
```


Mengembalikan enumerator untuk koleksi ini.

**Returns:**
java.util.Iterator&lt;com.aspose.tasks.Task&gt; - sebuah enumerator untuk koleksi ini.
### remove(Object item) {#remove-java.lang.Object-}
```
public final boolean remove(Object item)
```


Ini adalah implementasi stub dari metode Remove pada ICollection, yang hanya melempar UnsupportedOperationException.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| item | java.lang.Object | Item yang akan dihapus. |

**Returns:**
boolean - `true` jika item dihapus; `false` jika tidak.
### size() {#size--}
```
public final int size()
```


Mendapatkan jumlah objek yang terkandung dalam TaskCollection.

**Returns:**
int - jumlah objek yang terdapat dalam TaskCollection.
### sort(Comparator&lt;? super Task&gt; c) {#sort-java.util.Comparator---super-com.aspose.tasks.Task--}
```
public final void sort(Comparator<? super Task> c)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| c | java.util.Comparator&lt;? super com.aspose.tasks.Task&gt; | \{@inheritDoc\} |

### toList() {#toList--}
```
public final List<Task> toList()
```


Mengonversi objek TaskCollection menjadi daftar objek [Task](../../com.aspose.tasks/task).

**Returns:**
java.util.List&lt;com.aspose.tasks.Task&gt; - mengembalikan daftar yang berisi instance kelas [Task](../../com.aspose.tasks/task) dari koleksi ini.
