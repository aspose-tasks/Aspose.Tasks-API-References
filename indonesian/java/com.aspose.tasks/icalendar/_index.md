---
title: "ICalendar"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili abstraksi kalender yang dapat digunakan untuk berbagai perhitungan tanggal dan durasi."
type: docs
weight: 376
url: /id/java/com.aspose.tasks/icalendar/
---
```
public interface ICalendar
```

Mewakili abstraksi kalender yang dapat digunakan untuk berbagai perhitungan tanggal dan durasi.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getFinishDateByStartAndWork(Date start, Duration work)](#getFinishDateByStartAndWork-java.util.Date-com.aspose.tasks.Duration-) | Menghitung tanggal ketika jumlah waktu kerja yang ditentukan akan berlalu menurut kalender. |
| [getFinishDateByStartAndWork(Date start, double work)](#getFinishDateByStartAndWork-java.util.Date-double-) | Menghitung tanggal ketika jumlah waktu kerja yang ditentukan akan berlalu menurut kalender. |
| [getNextWorkingDayStart(Date date)](#getNextWorkingDayStart-java.util.Date-) | Menghitung awal hari kerja berikutnya untuk tanggal yang ditentukan. |
| [getPreviousWorkingDayEnd(Date date)](#getPreviousWorkingDayEnd-java.util.Date-) | Menghitung akhir tanggal kerja sebelumnya dari tanggal yang ditentukan. |
| [getStartDateFromFinishAndDuration(Date finish, Duration duration)](#getStartDateFromFinishAndDuration-java.util.Date-com.aspose.tasks.Duration-) | Mengembalikan tanggal mulai berdasarkan tanggal selesai dan durasi yang ditentukan. |
| [getStartDateFromFinishAndDuration(Date finish, double duration)](#getStartDateFromFinishAndDuration-java.util.Date-double-) | Mengembalikan tanggal mulai berdasarkan tanggal selesai dan durasi yang ditentukan. |
| [getTaskFinishDateFromDuration(Task task, double duration)](#getTaskFinishDateFromDuration-com.aspose.tasks.Task-double-) | Menghitung tanggal dan waktu selesai tugas dari tanggal mulai, bagian terpisah, dan durasi kerja. |
| [getWorkStart(Date date)](#getWorkStart-java.util.Date-) | Menghitung awal waktu kerja berikutnya mulai dari tanggal dan waktu yang ditentukan. |
| [getWorkingHours(Date dt)](#getWorkingHours-java.util.Date-) | Mengembalikan jumlah jam kerja pada tanggal yang ditentukan. |
| [getWorkingHours(Date start, Date finish)](#getWorkingHours-java.util.Date-java.util.Date-) | Kembalikan WorkUnit - Mulai, Selesai, dan Durasi jam kerja untuk interval tanggal dan waktu yang ditentukan. |
| [getWorkingHoursTimeSpan(Date start, Date finish)](#getWorkingHoursTimeSpan-java.util.Date-java.util.Date-) | Mengembalikan jumlah jam kerja antara tanggal yang ditentukan. |
| [getWorkingTimes(Date dt)](#getWorkingTimes-java.util.Date-) | Mengembalikan [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) dari waktu kerja untuk tanggal yang ditentukan. |
| [isDayWorking(Date dt)](#isDayWorking-java.util.Date-) | Menentukan apakah hari yang ditentukan adalah hari kerja menurut kalender. |
| [isEmpty()](#isEmpty--) | Mengembalikan apakah kalender tidak memiliki jam kerja yang didefinisikan. |
### getFinishDateByStartAndWork(Date start, Duration work) {#getFinishDateByStartAndWork-java.util.Date-com.aspose.tasks.Duration-}
```
public abstract Date getFinishDateByStartAndWork(Date start, Duration work)
```


Menghitung tanggal ketika jumlah waktu kerja yang ditentukan akan berlalu menurut kalender.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| mulai | java.util.Date | Tanggal mulai. |
| work | [Duration](../../com.aspose.tasks/duration) | Durasi kerja. |

**Returns:**
java.util.Date - Tanggal selesai.
### getFinishDateByStartAndWork(Date start, double work) {#getFinishDateByStartAndWork-java.util.Date-double-}
```
public abstract Date getFinishDateByStartAndWork(Date start, double work)
```


Menghitung tanggal ketika jumlah waktu kerja yang ditentukan akan berlalu menurut kalender.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| mulai | java.util.Date | Tanggal mulai. |
| kerja | double | Durasi kerja. |

**Returns:**
java.util.Date - Tanggal selesai.
### getNextWorkingDayStart(Date date) {#getNextWorkingDayStart-java.util.Date-}
```
public abstract Date getNextWorkingDayStart(Date date)
```


Menghitung awal hari kerja berikutnya untuk tanggal yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| tanggal | java.util.Date | Tanggal untuk mendapatkan awal hari kerja berikutnya. |

**Returns:**
java.util.Date - Awal hari kerja berikutnya System.DateTime.
### getPreviousWorkingDayEnd(Date date) {#getPreviousWorkingDayEnd-java.util.Date-}
```
public abstract Date getPreviousWorkingDayEnd(Date date)
```


Menghitung akhir tanggal kerja sebelumnya dari tanggal yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| tanggal | java.util.Date | tanggal untuk menghitung akhir hari kerja sebelumnya. |

**Returns:**
java.util.Date - Akhir hari kerja sebelumnya
### getStartDateFromFinishAndDuration(Date finish, Duration duration) {#getStartDateFromFinishAndDuration-java.util.Date-com.aspose.tasks.Duration-}
```
public abstract Date getStartDateFromFinishAndDuration(Date finish, Duration duration)
```


Mengembalikan tanggal mulai berdasarkan tanggal selesai dan durasi yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| selesai | java.util.Date | Tanggal selesai yang ditentukan. |
| duration | [Duration](../../com.aspose.tasks/duration) | Durasi yang ditentukan. |

**Returns:**
java.util.Date - Tanggal mulai yang dihitung.
### getStartDateFromFinishAndDuration(Date finish, double duration) {#getStartDateFromFinishAndDuration-java.util.Date-double-}
```
public abstract Date getStartDateFromFinishAndDuration(Date finish, double duration)
```


Mengembalikan tanggal mulai berdasarkan tanggal selesai dan durasi yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| selesai | java.util.Date | Tanggal selesai yang ditentukan. |
| durasi | double | Durasi yang ditentukan. |

**Returns:**
java.util.Date - Tanggal mulai yang dihitung.
### getTaskFinishDateFromDuration(Task task, double duration) {#getTaskFinishDateFromDuration-com.aspose.tasks.Task-double-}
```
public abstract Date getTaskFinishDateFromDuration(Task task, double duration)
```


Menghitung tanggal dan waktu selesai tugas dari tanggal mulai, bagian terpisah, dan durasi kerja.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Tugas untuk menghitung tanggal selesai. |
|  | durasi | double | Durasi untuk dihitung. |

Mengembalikan DateTime.MinValue jika tugas adalah ringkasan, null atau tanggal mulainya tidak diatur. |

**Returns:**
java.util.Date - Tanggal selesai tugas untuk tanggal mulai dan durasi yang diberikan.
### getWorkStart(Date date) {#getWorkStart-java.util.Date-}
```
public abstract Date getWorkStart(Date date)
```


Menghitung awal waktu kerja berikutnya mulai dari tanggal dan waktu yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| tanggal | java.util.Date | Tanggal dan waktu. |

**Returns:**
java.util.Date - Awal waktu kerja terdekat.
### getWorkingHours(Date dt) {#getWorkingHours-java.util.Date-}
```
public abstract double getWorkingHours(Date dt)
```


Mengembalikan jumlah jam kerja pada tanggal yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| dt | java.util.Date | Tanggal untuk mendapatkan jam kerja. |

**Returns:**
double - Jam kerja pada tanggal yang ditentukan.
### getWorkingHours(Date start, Date finish) {#getWorkingHours-java.util.Date-java.util.Date-}
```
public abstract WorkUnit getWorkingHours(Date start, Date finish)
```


Kembalikan WorkUnit - Mulai, Selesai, dan Durasi jam kerja untuk interval tanggal dan waktu yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| mulai | java.util.Date | Tanggal mulai interval. |
| selesai | java.util.Date | Tanggal selesai interval. |

**Returns:**
[WorkUnit](../../com.aspose.tasks/workunit) - Instance of [WorkUnit](../../com.aspose.tasks/workunit) class containing Start, Finish and Duration of working hours.
### getWorkingHoursTimeSpan(Date start, Date finish) {#getWorkingHoursTimeSpan-java.util.Date-java.util.Date-}
```
public abstract double getWorkingHoursTimeSpan(Date start, Date finish)
```


Mengembalikan jumlah jam kerja antara tanggal yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| mulai | java.util.Date | Tanggal mulai interval. |
| selesai | java.util.Date | Tanggal selesai interval. |

**Returns:**
double - Jumlah jam kerja menurut instance kalender.
### getWorkingTimes(Date dt) {#getWorkingTimes-java.util.Date-}
```
public abstract WorkingTimeCollection getWorkingTimes(Date dt)
```


Mengembalikan [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) dari waktu kerja untuk tanggal yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| dt | java.util.Date | Tanggal untuk mendapatkan waktu kerja. |

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - Collection of [WorkingTime](../../com.aspose.tasks/workingtime) instances.
### isDayWorking(Date dt) {#isDayWorking-java.util.Date-}
```
public abstract boolean isDayWorking(Date dt)
```


Menentukan apakah hari yang ditentukan adalah hari kerja menurut kalender.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| dt | java.util.Date | Tanggal untuk memeriksa apakah hari tersebut adalah hari kerja. |

**Returns:**
boolean - True jika hari tersebut adalah hari kerja.
### isEmpty() {#isEmpty--}
```
public abstract boolean isEmpty()
```


Mengembalikan apakah kalender tidak memiliki jam kerja yang didefinisikan.

**Returns:**
boolean - Benar jika kalender tidak memiliki jam kerja yang didefinisikan.
