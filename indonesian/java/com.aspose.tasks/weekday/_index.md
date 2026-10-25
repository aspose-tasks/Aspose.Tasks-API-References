---
title: "WeekDay"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili hari dalam seminggu yang dapat mendefinisikan hari reguler dalam seminggu atau hari pengecualian dalam kalender."
type: docs
weight: 352
url: /id/java/com.aspose.tasks/weekday/
---

**Inheritance:**
java.lang.Object
```
public class WeekDay
```

Mewakili hari dalam seminggu yang dapat mendefinisikan hari reguler dalam seminggu atau hari pengecualian dalam kalender.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [WeekDay(int dayType)](#WeekDay-int-) | Menginisialisasi instance baru dari kelas [WeekDay](../../com.aspose.tasks/weekday) dengan tipe hari yang ditentukan. |
| [WeekDay(int dayType, List&lt;WorkingTime&gt; workingTimes)](#WeekDay-int-java.util.List-com.aspose.tasks.WorkingTime--) | Menginisialisasi instance baru dari kelas [WeekDay](../../com.aspose.tasks/weekday) dengan tipe hari yang ditentukan dan daftar periode kerja. |
| [WeekDay(int dayType, WorkingTime[] workingTimes)](#WeekDay-int-com.aspose.tasks.WorkingTime...-) | Menginisialisasi instance baru dari kelas [WeekDay](../../com.aspose.tasks/weekday) dengan tipe hari yang ditentukan serta periode kerja. |
| [WeekDay()](#WeekDay--) | Menginisialisasi instance baru dari kelas [WeekDay](../../com.aspose.tasks/weekday). |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [castToDayType(int dw)](#castToDayType-int-) | Mengubah tipe .Net's [DayOfWeek](../../com.aspose.tasks/dayofweek) menjadi `DayType`([getDayType()](../../com.aspose.tasks/weekday\#getDayType--)/[setDayType(int)](../../com.aspose.tasks/weekday\#setDayType-int-)). |
| [createDefaultWorkingDay(int dayType)](#createDefaultWorkingDay-int-) | Membuat hari kerja default. |
| [deepClone()](#deepClone--) | Mengembalikan salinan mendalam dari hari dalam minggu. |
| [equals(Object obj)](#equals-java.lang.Object-) | Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| [getDayType()](#getDayType--) | Mendapatkan tipe hari. |
| [getDayWorking()](#getDayWorking--) | Mendapatkan nilai yang menunjukkan apakah tanggal atau tipe hari yang ditentukan merupakan hari kerja. |
| [getFromDate()](#getFromDate--) | Mendapatkan awal waktu pengecualian. |
| [getToDate()](#getToDate--) | Mendapatkan akhir waktu pengecualian. |
| [getWorkingTime()](#getWorkingTime--) | Mengembalikan waktu kerja untuk hari dalam minggu. |
| [getWorkingTimes()](#getWorkingTimes--) | Mendapatkan WorkingTimeCollection untuk instance WeekDay ini. |
| [hashCode()](#hashCode--) | Mengembalikan nilai kode hash untuk instance kelas [WeekDay](../../com.aspose.tasks/weekday). |
| [setDayWorking(boolean value)](#setDayWorking-boolean-) | Mengatur nilai yang menunjukkan apakah tanggal atau tipe hari yang ditentukan merupakan hari kerja. |
| [setDefaultWorkingTime(WeekDay day)](#setDefaultWorkingTime-com.aspose.tasks.WeekDay-) | Mengatur periode waktu default untuk hari dalam minggu yang ditentukan. |
| [setFromDate(Date value)](#setFromDate-java.util.Date-) | Mengatur awal waktu pengecualian. |
| [setToDate(Date value)](#setToDate-java.util.Date-) | Mengatur akhir waktu pengecualian. |
### WeekDay(int dayType) {#WeekDay-int-}
```
public WeekDay(int dayType)
```


Menginisialisasi instance baru dari kelas [WeekDay](../../com.aspose.tasks/weekday) dengan tipe hari yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| dayType | int | Tipe hari yang ditentukan. |

### WeekDay(int dayType, List&lt;WorkingTime&gt; workingTimes) {#WeekDay-int-java.util.List-com.aspose.tasks.WorkingTime--}
```
public WeekDay(int dayType, List<WorkingTime> workingTimes)
```


Menginisialisasi instance baru dari kelas [WeekDay](../../com.aspose.tasks/weekday) dengan tipe hari yang ditentukan dan daftar periode kerja.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| dayType | int | Tipe hari yang ditentukan. |
| workingTimes | java.util.List&lt;com.aspose.tasks.WorkingTime&gt; | Daftar periode waktu kerja. |

### WeekDay(int dayType, WorkingTime[] workingTimes) {#WeekDay-int-com.aspose.tasks.WorkingTime...-}
```
public WeekDay(int dayType, WorkingTime[] workingTimes)
```


Menginisialisasi instance baru dari kelas [WeekDay](../../com.aspose.tasks/weekday) dengan tipe hari yang ditentukan serta periode kerja.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| dayType | int | Tipe hari yang ditentukan. |
| workingTimes | [WorkingTime\[\]](../../com.aspose.tasks/workingtime) | Array periode waktu kerja. |

### WeekDay() {#WeekDay--}
```
public WeekDay()
```


Menginisialisasi instance baru dari kelas [WeekDay](../../com.aspose.tasks/weekday).

### castToDayType(int dw) {#castToDayType-int-}
```
public static int castToDayType(int dw)
```


Mengubah tipe .Net's [DayOfWeek](../../com.aspose.tasks/dayofweek) menjadi `DayType`([getDayType()](../../com.aspose.tasks/weekday\#getDayType--)/[setDayType(int)](../../com.aspose.tasks/weekday\#setDayType-int-)).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| dw | int | Hari dalam minggu yang akan dikonversi. |

**Returns:**
int - Tipe hari hasil konversi.
### createDefaultWorkingDay(int dayType) {#createDefaultWorkingDay-int-}
```
public static WeekDay createDefaultWorkingDay(int dayType)
```


Membuat hari kerja default.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| dayType | int | Tipe hari untuk membuat hari kerja default. |

**Returns:**
[WeekDay](../../com.aspose.tasks/weekday) - A default working day with working times 8-12 and 13-17.
### deepClone() {#deepClone--}
```
public final WeekDay deepClone()
```


Mengembalikan salinan mendalam dari hari dalam minggu.

**Returns:**
[WeekDay](../../com.aspose.tasks/weekday) - Returns the deep copy of the week day.
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
boolean - **True** jika objek yang ditentukan adalah WeekDay yang memiliki nilai FromDate, ToDate, dan WorkingTimes yang sama dengan instance ini; jika tidak, **false**.
### getDayType() {#getDayType--}
```
public final int getDayType()
```


Mendapatkan tipe hari.

**Returns:**
int - tipe hari.
### getDayWorking() {#getDayWorking--}
```
public final boolean getDayWorking()
```


Mendapatkan nilai yang menunjukkan apakah tanggal atau tipe hari yang ditentukan merupakan hari kerja.

**Returns:**
boolean - nilai yang menunjukkan apakah tanggal atau tipe hari yang ditentukan sedang bekerja.
### getFromDate() {#getFromDate--}
```
public final Date getFromDate()
```


Mendapatkan awal waktu pengecualian.

**Returns:**
java.util.Date - awal waktu pengecualian.
### getToDate() {#getToDate--}
```
public final Date getToDate()
```


Mendapatkan akhir waktu pengecualian.

**Returns:**
java.util.Date - akhir waktu pengecualian.
### getWorkingTime() {#getWorkingTime--}
```
public final double getWorkingTime()
```


Mengembalikan waktu kerja untuk hari dalam minggu.

**Returns:**
double - Waktu kerja.
### getWorkingTimes() {#getWorkingTimes--}
```
public final WorkingTimeCollection getWorkingTimes()
```


Mengambil WorkingTimeCollection untuk instance WeekDay ini. Koleksi waktu kerja yang mendefinisikan waktu yang dikerjakan pada hari kerja.

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - WorkingTimeCollection for this WeekDay instance.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Mengembalikan nilai kode hash untuk instance kelas [WeekDay](../../com.aspose.tasks/weekday).

**Returns:**
int - mengembalikan nilai kode hash untuk objek ini.
### setDayWorking(boolean value) {#setDayWorking-boolean-}
```
public final void setDayWorking(boolean value)
```


Mengatur nilai yang menunjukkan apakah tanggal atau tipe hari yang ditentukan merupakan hari kerja.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah tanggal atau tipe hari yang ditentukan sedang bekerja. |

### setDefaultWorkingTime(WeekDay day) {#setDefaultWorkingTime-com.aspose.tasks.WeekDay-}
```
public static void setDefaultWorkingTime(WeekDay day)
```


Mengatur periode waktu default untuk hari dalam minggu yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| day | [WeekDay](../../com.aspose.tasks/weekday) | Hari minggu untuk menetapkan hari kerja default. |

### setFromDate(Date value) {#setFromDate-java.util.Date-}
```
public final void setFromDate(Date value)
```


Mengatur awal waktu pengecualian.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date | awal waktu pengecualian. |

### setToDate(Date value) {#setToDate-java.util.Date-}
```
public final void setToDate(Date value)
```


Mengatur akhir waktu pengecualian.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date | akhir waktu pengecualian. |

