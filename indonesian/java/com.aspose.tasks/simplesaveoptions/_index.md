---
title: "SimpleSaveOptions"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Ini adalah kelas dasar abstrak yang memungkinkan pengguna menentukan opsi dasar saat menyimpan proyek ke format tertentu."
type: docs
weight: 277
url: /id/java/com.aspose.tasks/simplesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class SimpleSaveOptions
```

Ini adalah kelas dasar abstrak yang memungkinkan pengguna menentukan opsi dasar saat menyimpan proyek ke format tertentu.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [SimpleSaveOptions()](#SimpleSaveOptions--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getSaveFormat()](#getSaveFormat--) | Mendapatkan format di mana dokumen akan disimpan jika objek opsi penyimpanan ini digunakan. |
| [getTasksComparer()](#getTasksComparer--) | Mendapatkan pembanding untuk mengurutkan tugas pada diagram Gantt dan diagram Lembar Tugas. |
| [getTasksFilter()](#getTasksFilter--) | Mendapatkan kondisi yang digunakan untuk menyaring tugas yang ditampilkan pada diagram Gantt, Lembar Tugas, dan Penggunaan Tugas. |
| [setTasksComparer(Comparator&lt;Task&gt; value)](#setTasksComparer-java.util.Comparator-com.aspose.tasks.Task--) | Mengatur pembanding untuk mengurutkan tugas pada diagram Gantt dan diagram Lembar Tugas. |
| [setTasksFilter(ICondition&lt;Task&gt; value)](#setTasksFilter-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | Mengatur kondisi yang digunakan untuk menyaring tugas yang ditampilkan pada diagram Gantt, Lembar Tugas, dan Penggunaan Tugas. |
### SimpleSaveOptions() {#SimpleSaveOptions--}
```
public SimpleSaveOptions()
```


### getSaveFormat() {#getSaveFormat--}
```
public final int getSaveFormat()
```


Mendapatkan format di mana dokumen akan disimpan jika objek opsi penyimpanan ini digunakan.

**Returns:**
int - [SaveFileFormat](../../com.aspose.tasks/savefileformat) di mana dokumen akan disimpan.
### getTasksComparer() {#getTasksComparer--}
```
public final Comparator<Task> getTasksComparer()
```


Mendapatkan pembanding untuk mengurutkan tugas pada diagram Gantt dan diagram Lembar Tugas.

**Returns:**
java.util.Comparator&lt;com.aspose.tasks.Task&gt; - pembanding untuk mengurutkan tugas pada diagram Gantt dan diagram Lembar Tugas.
### getTasksFilter() {#getTasksFilter--}
```
public final ICondition<Task> getTasksFilter()
```


Mendapatkan kondisi yang digunakan untuk menyaring tugas yang ditampilkan pada diagram Gantt, Lembar Tugas, dan Penggunaan Tugas.

--------------------

Jika nilai tidak ditentukan, filter default digunakan yang menghapus tugas yang tidak terlihat -- yaitu tugas turunan dari tugas yang dikompresi.

**Returns:**
[ICondition](../../com.aspose.tasks/icondition) - the condition which is used to filter tasks rendered on Gantt, Task Sheet and Task Usage charts.
### setTasksComparer(Comparator&lt;Task&gt; value) {#setTasksComparer-java.util.Comparator-com.aspose.tasks.Task--}
```
public final void setTasksComparer(Comparator<Task> value)
```


Mengatur pembanding untuk mengurutkan tugas pada diagram Gantt dan diagram Lembar Tugas.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Comparator&lt;com.aspose.tasks.Task&gt; | pembanding untuk mengurutkan tugas pada diagram Gantt dan diagram Lembar Tugas. |

### setTasksFilter(ICondition&lt;Task&gt; value) {#setTasksFilter-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public final void setTasksFilter(ICondition<Task> value)
```


Mengatur kondisi yang digunakan untuk menyaring tugas yang ditampilkan pada diagram Gantt, Lembar Tugas, dan Penggunaan Tugas.

--------------------

Jika nilai tidak ditentukan, filter default digunakan yang menghapus tugas yang tidak terlihat -- yaitu tugas turunan dari tugas yang dikompresi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | kondisi yang digunakan untuk menyaring tugas yang dirender pada diagram Gantt, Lembar Tugas, dan Penggunaan Tugas. |

