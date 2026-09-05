---
title: "WorkingTime"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili waktu kerja selama hari kerja."
type: docs
weight: 365
url: /id/java/com.aspose.tasks/workingtime/
---

**Inheritance:**
java.lang.Object
```
public class WorkingTime
```

Mewakili waktu kerja selama hari kerja.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [WorkingTime(Date fromTime, Date toTime)](#WorkingTime-java.util.Date-java.util.Date-) | Menginisialisasi sebuah instance baru dari kelas [WorkingTime](../../com.aspose.tasks/workingtime) dengan interval dengan waktu mulai dan selesai yang ditentukan. |
| [WorkingTime(double fromTime, double toTime)](#WorkingTime-double-double-) | Menginisialisasi sebuah instance baru dari kelas [WorkingTime](../../com.aspose.tasks/workingtime) dengan item interval dengan waktu mulai dan selesai yang ditentukan. |
| [WorkingTime(int fromHours, int toHours)](#WorkingTime-int-int-) | Menginisialisasi sebuah instance baru dari kelas [WorkingTime](../../com.aspose.tasks/workingtime) dengan item interval dengan waktu mulai dan selesai yang ditentukan. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | Memeriksa bahwa objek-objek tersebut sama. |
| [getFrom()](#getFrom--) | Mendapatkan awal dari waktu kerja. |
| [getTo()](#getTo--) | Mendapatkan akhir dari waktu kerja. |
| [hashCode()](#hashCode--) | Mengembalikan nilai kode hash untuk instance dari kelas [WorkingTime](../../com.aspose.tasks/workingtime). |
### WorkingTime(Date fromTime, Date toTime) {#WorkingTime-java.util.Date-java.util.Date-}
```
public WorkingTime(Date fromTime, Date toTime)
```


Menginisialisasi sebuah instance baru dari kelas [WorkingTime](../../com.aspose.tasks/workingtime) dengan interval dengan waktu mulai dan selesai yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fromTime | java.util.Date | waktu mulai interval |
| toTime | java.util.Date | waktu akhir interval |

### WorkingTime(double fromTime, double toTime) {#WorkingTime-double-double-}
```
public WorkingTime(double fromTime, double toTime)
```


Menginisialisasi sebuah instance baru dari kelas [WorkingTime](../../com.aspose.tasks/workingtime) dengan item interval dengan waktu mulai dan selesai yang ditentukan.

--------------------

&gt; ```
&gt; Overload dari ctor WorkingTime dapat digunakan untuk menginisialisasi awal dan akhir interval menggunakan TimeSpan:
&gt; ``````

 [C#]
var wt = new WorkingTime(new TimeSpan(9, 0, 0), new TimeSpan(18, 0, 0));
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fromTime | double | Interval's start time represented by double struct. |
| toTime | double | Interval's end time represented by double struct. |

### WorkingTime(int fromHours, int toHours) {#WorkingTime-int-int-}
```
public WorkingTime(int fromHours, int toHours)
```


Initializes a new instance of the [WorkingTime](../../com.aspose.tasks/workingtime) class with an interval item with the specified start and finish times.

--------------------

&gt; ```
&gt; The overload of WorkingTime ctor can be used to initialize interval's start and end using whole hours:
&gt; ``````

 [C#]
 var wt = new WorkingTime(9, 13);
 
```



**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fromHours | int | Waktu mulai interval yang direpresentasikan oleh bilangan bulat jam (0-24). |
| toHours | int | Waktu akhir interval yang direpresentasikan oleh bilangan bulat jam (0-24). |

### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Memeriksa bahwa objek-objek tersebut sama.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| obj | java.lang.Object | Objek kedua untuk dibandingkan. |

**Returns:**
boolean - True jika objek-objek tersebut sama, false jika tidak.
### getFrom() {#getFrom--}
```
public final Date getFrom()
```


Mendapatkan awal dari waktu kerja.

**Returns:**
java.util.Date - awal dari waktu kerja.
### getTo() {#getTo--}
```
public final Date getTo()
```


Mendapatkan akhir dari waktu kerja.

**Returns:**
java.util.Date - akhir dari waktu kerja.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Mengembalikan nilai kode hash untuk instance dari kelas [WorkingTime](../../com.aspose.tasks/workingtime).

**Returns:**
int - mengembalikan nilai kode hash untuk objek ini.
