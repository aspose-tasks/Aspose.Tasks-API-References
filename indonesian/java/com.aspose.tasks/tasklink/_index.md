---
title: "TaskLink"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili tautan pendahulu."
type: docs
weight: 295
url: /id/java/com.aspose.tasks/tasklink/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.IEquatable
```
public final class TaskLink implements System.IEquatable<TaskLink>
```

Mewakili tautan pendahulu.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [equals(TaskLink other)](#equals-com.aspose.tasks.TaskLink-) | Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| [equals(Object obj)](#equals-java.lang.Object-) | Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| [getCrossProjectName()](#getCrossProjectName--) | Mendapatkan proyek predecessor eksternal. |
| [getLagFormat()](#getLagFormat--) | Mendapatkan format untuk mengekspresikan format lag. |
| [getLinkLag()](#getLinkLag--) | Mendapatkan lag dalam sepersepuluh menit atau persentase. |
| [getLinkLagTimeSpan()](#getLinkLagTimeSpan--) | Mendapatkan durasi lag, tergantung pada LagFormat. |
| [getLinkType()](#getLinkType--) | Mendapatkan tipe tautan. |
| [getPredTask()](#getPredTask--) | Mendapatkan tugas predecessor. |
| [getSuccTask()](#getSuccTask--) | Mendapatkan tugas successor. |
| [hashCode()](#hashCode--) | Mengembalikan nilai kode hash untuk instance kelas [TaskLink](../../com.aspose.tasks/tasklink). |
| [isCrossProject()](#isCrossProject--) | Mendapatkan nilai yang menunjukkan apakah predecessor merupakan bagian dari proyek lain. |
| [setCrossProject(boolean value)](#setCrossProject-boolean-) | Mengatur nilai yang menunjukkan apakah predecessor merupakan bagian dari proyek lain. |
| [setCrossProjectName(String value)](#setCrossProjectName-java.lang.String-) | Mengatur proyek predecessor eksternal. |
| [setLagFormat(byte value)](#setLagFormat-byte-) | Mengatur format untuk mengekspresikan format lag. |
| [setLinkLag(int value)](#setLinkLag-int-) | Mengatur lag dalam sepersepuluh menit atau persentase. |
| [setLinkLagTimeSpan(double value)](#setLinkLagTimeSpan-double-) | Mengatur durasi lag, tergantung pada LagFormat. |
| [setLinkType(int value)](#setLinkType-int-) | Mengatur tipe tautan. |
| [setPredTask(Task value)](#setPredTask-com.aspose.tasks.Task-) | Mengatur tugas predecessor. |
| [setSuccTask(Task value)](#setSuccTask-com.aspose.tasks.Task-) | Mengatur tugas successor. |
| [toString()](#toString--) | Mengembalikan representasi string dari TaskLink. |
### equals(TaskLink other) {#equals-com.aspose.tasks.TaskLink-}
```
public final boolean equals(TaskLink other)
```


Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| other | [TaskLink](../../com.aspose.tasks/tasklink) | Instance yang ditentukan dari kelas [TaskLink](../../com.aspose.tasks/tasklink) untuk dibandingkan dengan instance ini. |

**Returns:**
boolean - **True** jika instance yang ditentukan dari kelas [TaskLink](../../com.aspose.tasks/tasklink) memiliki predecessor dan successor yang sama dengan instance ini; jika tidak, **false**.
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
boolean - **True** jika objek yang ditentukan adalah TaskLink yang memiliki predecessor dan successor yang sama dengan instance ini; jika tidak, **false**.
### getCrossProjectName() {#getCrossProjectName--}
```
public final String getCrossProjectName()
```


Mendapatkan proyek predecessor eksternal.

**Returns:**
java.lang.String - proyek predecessor eksternal.
### getLagFormat() {#getLagFormat--}
```
public final byte getLagFormat()
```


Mendapatkan format untuk mengekspresikan format lag.

**Returns:**
byte - format untuk mengekspresikan format lag.
### getLinkLag() {#getLinkLag--}
```
public final int getLinkLag()
```


Mendapatkan lag dalam sepersepuluh menit atau persentase.

**Returns:**
int - lag dalam sepersepuluh menit atau persentase.
### getLinkLagTimeSpan() {#getLinkLagTimeSpan--}
```
public final double getLinkLagTimeSpan()
```


Mendapatkan durasi lag, tergantung pada LagFormat.

**Returns:**
double - durasi lag, tergantung pada LagFormat.
### getLinkType() {#getLinkType--}
```
public final int getLinkType()
```


Mendapatkan tipe tautan.

**Returns:**
int - tipe dari sebuah link.
### getPredTask() {#getPredTask--}
```
public final Task getPredTask()
```


Mendapatkan tugas predecessor.

**Returns:**
[Task](../../com.aspose.tasks/task) - the predecessor task.
### getSuccTask() {#getSuccTask--}
```
public final Task getSuccTask()
```


Mendapatkan tugas successor.

**Returns:**
[Task](../../com.aspose.tasks/task) - the successor task.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Mengembalikan nilai kode hash untuk instance kelas [TaskLink](../../com.aspose.tasks/tasklink).

**Returns:**
int - mengembalikan nilai kode hash untuk objek ini.
### isCrossProject() {#isCrossProject--}
```
public final boolean isCrossProject()
```


Mendapatkan nilai yang menunjukkan apakah predecessor merupakan bagian dari proyek lain.

**Returns:**
boolean - nilai yang menunjukkan apakah sebuah predecessor merupakan bagian dari proyek lain.
### setCrossProject(boolean value) {#setCrossProject-boolean-}
```
public final void setCrossProject(boolean value)
```


Mengatur nilai yang menunjukkan apakah predecessor merupakan bagian dari proyek lain.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah sebuah predecessor merupakan bagian dari proyek lain. |

### setCrossProjectName(String value) {#setCrossProjectName-java.lang.String-}
```
public final void setCrossProjectName(String value)
```


Mengatur proyek predecessor eksternal.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | proyek predecessor eksternal. |

### setLagFormat(byte value) {#setLagFormat-byte-}
```
public final void setLagFormat(byte value)
```


Mengatur format untuk mengekspresikan format lag.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | byte | format untuk mengekspresikan format lag. |

### setLinkLag(int value) {#setLinkLag-int-}
```
public final void setLinkLag(int value)
```


Mengatur lag dalam sepersepuluh menit atau persentase.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | lag dalam sepersepuluh menit atau persentase. |

### setLinkLagTimeSpan(double value) {#setLinkLagTimeSpan-double-}
```
public final void setLinkLagTimeSpan(double value)
```


Mengatur durasi lag, tergantung pada LagFormat.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | double | durasi lag, tergantung pada LagFormat. |

### setLinkType(int value) {#setLinkType-int-}
```
public final void setLinkType(int value)
```


Mengatur tipe tautan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | tipe dari sebuah link. |

### setPredTask(Task value) {#setPredTask-com.aspose.tasks.Task-}
```
public final void setPredTask(Task value)
```


Mengatur tugas predecessor.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | tugas predecessor. |

### setSuccTask(Task value) {#setSuccTask-com.aspose.tasks.Task-}
```
public final void setSuccTask(Task value)
```


Mengatur tugas successor.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [Task](../../com.aspose.tasks/task) | tugas successor. |

### toString() {#toString--}
```
public String toString()
```


Mengembalikan representasi string dari sebuah TaskLink. Detail tepat dari representasi tidak ditentukan dan dapat berubah.

**Returns:**
java.lang.String - string yang merepresentasikan objek TaskLink.
