---
title: "TaskBaseline"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili Baseline dari sebuah Tugas."
type: docs
weight: 291
url: /id/java/com.aspose.tasks/taskbaseline/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.Baseline](../../com.aspose.tasks/baseline)

**All Implemented Interfaces:**
java.lang.Comparable
```
public class TaskBaseline extends Baseline implements Comparable<Baseline>
```

Mewakili Baseline dari sebuah Tugas.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [TaskBaseline(Task task)](#TaskBaseline-com.aspose.tasks.Task-) | Menginisialisasi instance baru dari kelas [TaskBaseline](../../com.aspose.tasks/taskbaseline). |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [compareTo(TaskBaseline other)](#compareTo-com.aspose.tasks.TaskBaseline-) | Implementasi antarmuka IComparable. |
| [equals(TaskBaseline other)](#equals-com.aspose.tasks.TaskBaseline-) | Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek TaskBaseline yang ditentukan. |
| [equals(Object obj)](#equals-java.lang.Object-) | Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| [getDuration()](#getDuration--) | Mendapatkan durasi terjadwal tugas saat baseline disimpan. |
| [getEstimatedDuration()](#getEstimatedDuration--) | Mendapatkan nilai yang menunjukkan apakah durasi baseline tugas diperkirakan. |
| [getFinish()](#getFinish--) | Mendapatkan tanggal selesai terjadwal tugas saat baseline disimpan. |
| [getFixedCost()](#getFixedCost--) | Mendapatkan biaya tetap tugas saat baseline disimpan. |
| [getInterim()](#getInterim--) | Mendapatkan nilai yang menunjukkan apakah ini adalah Baseline Interim. |
| [getStart()](#getStart--) | Mendapatkan tanggal mulai terjadwal tugas saat baseline disimpan. |
| [getTimephasedData()](#getTimephasedData--) | Mendapatkan instance TimephasedDataCollection untuk objek ini. |
| [hashCode()](#hashCode--) | Mengembalikan nilai kode hash untuk instance kelas [TaskBaseline](../../com.aspose.tasks/taskbaseline). |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Mengatur durasi terjadwal tugas saat baseline disimpan. |
| [setEstimatedDuration(boolean value)](#setEstimatedDuration-boolean-) | Mengatur nilai yang menunjukkan apakah durasi baseline tugas diperkirakan. |
| [setFinish(Date value)](#setFinish-java.util.Date-) | Mengatur tanggal selesai terjadwal tugas saat baseline disimpan. |
| [setFixedCost(double value)](#setFixedCost-double-) | Menetapkan biaya tetap tugas ketika baseline disimpan. |
| [setInterim(boolean value)](#setInterim-boolean-) | Menetapkan nilai yang menunjukkan apakah ini adalah Baseline Interim. |
| [setStart(Date value)](#setStart-java.util.Date-) | Menetapkan tanggal mulai terjadwal tugas ketika baseline disimpan. |
| [setTimephasedData(TimephasedDataCollection value)](#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-) | Menetapkan instance TimephasedDataCollection untuk objek ini. |
### TaskBaseline(Task task) {#TaskBaseline-com.aspose.tasks.Task-}
```
public TaskBaseline(Task task)
```


Menginisialisasi instance baru dari kelas [TaskBaseline](../../com.aspose.tasks/taskbaseline).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Tugas induk Baseline. |

### compareTo(TaskBaseline other) {#compareTo-com.aspose.tasks.TaskBaseline-}
```
public final int compareTo(TaskBaseline other)
```


Implementasi antarmuka IComparable. Membandingkan instance ini dengan objek Baseline yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| other | [TaskBaseline](../../com.aspose.tasks/taskbaseline) | objek Baseline yang ditentukan untuk dibandingkan dengan instance ini. |

**Returns:**
int - mengembalikan -1 jika instance ini kurang dari objek yang ditentukan, 1 jika instance ini lebih besar dari objek yang ditentukan; jika tidak mengembalikan 0
### equals(TaskBaseline other) {#equals-com.aspose.tasks.TaskBaseline-}
```
public final boolean equals(TaskBaseline other)
```


Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek TaskBaseline yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| other | [TaskBaseline](../../com.aspose.tasks/taskbaseline) | objek AssignmentBaseline yang ditentukan untuk dibandingkan dengan instance ini. |

**Returns:**
boolean - mengembalikan true jika instance ini sama dengan objek TaskBaseline yang ditentukan; jika tidak, false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| obj | java.lang.Object | Objek untuk dibandingkan dengan instance ini. |

**Returns:**
boolean - **True** jika objek yang ditentukan adalah TaskBaseline yang memiliki nilai UID yang sama dengan instance ini; jika tidak, **false**.
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Mendapatkan durasi terjadwal tugas saat baseline disimpan.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the scheduled duration of the task when the baseline was saved.
### getEstimatedDuration() {#getEstimatedDuration--}
```
public final boolean getEstimatedDuration()
```


Mendapatkan nilai yang menunjukkan apakah durasi baseline tugas diperkirakan.

**Returns:**
boolean - nilai yang menunjukkan apakah durasi baseline tugas diperkirakan.
### getFinish() {#getFinish--}
```
public final Date getFinish()
```


Mendapatkan tanggal selesai terjadwal tugas saat baseline disimpan.

**Returns:**
java.util.Date - tanggal selesai terjadwal tugas ketika baseline disimpan.
### getFixedCost() {#getFixedCost--}
```
public final double getFixedCost()
```


Mendapatkan biaya tetap tugas saat baseline disimpan.

**Returns:**
double - biaya tetap tugas ketika baseline disimpan.
### getInterim() {#getInterim--}
```
public final boolean getInterim()
```


Mendapatkan nilai yang menunjukkan apakah ini adalah Baseline Interim.

**Returns:**
boolean - nilai yang menunjukkan apakah ini adalah Baseline Interim.
### getStart() {#getStart--}
```
public final Date getStart()
```


Mendapatkan tanggal mulai terjadwal tugas saat baseline disimpan.

**Returns:**
java.util.Date - tanggal mulai terjadwal tugas ketika baseline disimpan.
### getTimephasedData() {#getTimephasedData--}
```
public final TimephasedDataCollection getTimephasedData()
```


Mendapatkan instance TimephasedDataCollection untuk objek ini. Data berfase waktu yang terkait dengan baseline tugas.

**Returns:**
[TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) - a TimephasedDataCollection instance for this object.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Mengembalikan nilai kode hash untuk instance kelas [TaskBaseline](../../com.aspose.tasks/taskbaseline).

**Returns:**
int - mengembalikan nilai kode hash untuk objek ini.
### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Mengatur durasi terjadwal tugas saat baseline disimpan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | durasi terjadwal tugas ketika baseline disimpan. |

### setEstimatedDuration(boolean value) {#setEstimatedDuration-boolean-}
```
public final void setEstimatedDuration(boolean value)
```


Mengatur nilai yang menunjukkan apakah durasi baseline tugas diperkirakan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah durasi baseline tugas diperkirakan. |

### setFinish(Date value) {#setFinish-java.util.Date-}
```
public final void setFinish(Date value)
```


Mengatur tanggal selesai terjadwal tugas saat baseline disimpan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date | tanggal selesai terjadwal tugas ketika baseline disimpan. |

### setFixedCost(double value) {#setFixedCost-double-}
```
public final void setFixedCost(double value)
```


Menetapkan biaya tetap tugas ketika baseline disimpan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | double | biaya tetap tugas ketika baseline disimpan. |

### setInterim(boolean value) {#setInterim-boolean-}
```
public final void setInterim(boolean value)
```


Menetapkan nilai yang menunjukkan apakah ini adalah Baseline Interim.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah ini adalah Baseline Interim. |

### setStart(Date value) {#setStart-java.util.Date-}
```
public final void setStart(Date value)
```


Menetapkan tanggal mulai terjadwal tugas ketika baseline disimpan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date | tanggal mulai terjadwal tugas ketika baseline disimpan. |

### setTimephasedData(TimephasedDataCollection value) {#setTimephasedData-com.aspose.tasks.TimephasedDataCollection-}
```
public final void setTimephasedData(TimephasedDataCollection value)
```


Menetapkan instance TimephasedDataCollection untuk objek ini. Data berfase waktu yang terkait dengan baseline tugas.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [TimephasedDataCollection](../../com.aspose.tasks/timephaseddatacollection) | instance TimephasedDataCollection untuk objek ini. |

