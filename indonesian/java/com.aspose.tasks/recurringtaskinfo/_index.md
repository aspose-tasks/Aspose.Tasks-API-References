---
title: "RecurringTaskInfo"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili detail tugas berulang dalam sebuah proyek."
type: docs
weight: 244
url: /id/java/com.aspose.tasks/recurringtaskinfo/
---

**Inheritance:**
java.lang.Object
```
public class RecurringTaskInfo
```

Mewakili detail tugas berulang dalam sebuah proyek.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getDailyRepetitions()](#getDailyRepetitions--) | Mendapatkan jumlah pengulangan untuk pola berulang harian. |
| [getDailyUseWorkdays()](#getDailyUseWorkdays--) | Mendapatkan nilai yang menunjukkan apakah akan menggunakan hari kerja untuk pola berulang harian. |
| [getDuration()](#getDuration--) | Mendapatkan durasi untuk satu kejadian tugas berulang. |
| [getEndDate()](#getEndDate--) | Mendapatkan tanggal berakhirnya kejadian. |
| [getMonthlyDay()](#getMonthlyDay--) | Mendapatkan jumlah hari dari pola berulang bulanan. |
| [getMonthlyOrdinalDay()](#getMonthlyOrdinalDay--) | Mendapatkan hari dari pola berulang bulanan saat menggunakan hari ordinal. |
| [getMonthlyOrdinalNumber()](#getMonthlyOrdinalNumber--) | Mendapatkan nomor ordinal dari pola berulang bulanan. |
| [getMonthlyOrdinalRepetitions()](#getMonthlyOrdinalRepetitions--) | Mendapatkan jumlah pengulangan untuk pola berulang bulanan saat menggunakan hari ordinal. |
| [getMonthlyRepetitions()](#getMonthlyRepetitions--) | Mendapatkan jumlah pengulangan untuk pola berulang bulanan. |
| [getMonthlyUseOrdinalDay()](#getMonthlyUseOrdinalDay--) | Mendapatkan nilai yang menunjukkan apakah akan menggunakan hari ordinal untuk pola berulang bulanan. |
| [getOccurrences()](#getOccurrences--) | Mendapatkan jumlah kejadian tugas berulang. |
| [getRecurrencePattern()](#getRecurrencePattern--) | Mendapatkan pola berulang dari tugas berulang. |
| [getStartDate()](#getStartDate--) | Mendapatkan tanggal mulai kejadian. |
| [getTask()](#getTask--) | Mendapatkan tugas induk dari instance kelas [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo) ini. |
| [getUseEndDate()](#getUseEndDate--) | Mendapatkan nilai yang menunjukkan apakah akan menggunakan tanggal akhir atau jumlah kejadian untuk tugas berulang. |
| [getWeeklyDays()](#getWeeklyDays--) | Mendapatkan kumpulan hari yang digunakan dalam pola berulang mingguan. |
| [getWeeklyRepetitions()](#getWeeklyRepetitions--) | Mendapatkan jumlah pengulangan untuk pola berulang mingguan. |
| [getYearlyDate()](#getYearlyDate--) | Mendapatkan tanggal untuk pola berulang tahunan. |
| [getYearlyOrdinalDay()](#getYearlyOrdinalDay--) | Mendapatkan hari kerja dari pola pengulangan tahunan saat menggunakan hari ordinal. |
| [getYearlyOrdinalMonth()](#getYearlyOrdinalMonth--) | Mendapatkan bulan dari pola pengulangan tahunan saat menggunakan hari ordinal. |
| [getYearlyOrdinalNumber()](#getYearlyOrdinalNumber--) | Mendapatkan nomor ordinal dari pola pengulangan tahunan. |
| [getYearlyUseOrdinalDay()](#getYearlyUseOrdinalDay--) | Mendapatkan nilai yang menunjukkan apakah akan menggunakan hari ordinal untuk pola pengulangan tahunan. |
| [setDailyRepetitions(int value)](#setDailyRepetitions-int-) | Mengatur jumlah pengulangan untuk pola pengulangan harian. |
| [setDailyUseWorkdays(boolean value)](#setDailyUseWorkdays-boolean-) | Mengatur nilai yang menunjukkan apakah akan menggunakan hari kerja untuk pola pengulangan harian. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Mengatur durasi untuk satu kejadian dari tugas berulang. |
| [setEndDate(Date value)](#setEndDate-java.util.Date-) | Mengatur tanggal berakhirnya kejadian. |
| [setMonthlyDay(int value)](#setMonthlyDay-int-) | Mengatur jumlah hari dari pola pengulangan bulanan. |
| [setMonthlyOrdinalDay(int value)](#setMonthlyOrdinalDay-int-) | Mengatur hari dari pola pengulangan bulanan saat menggunakan hari ordinal. |
| [setMonthlyOrdinalNumber(int value)](#setMonthlyOrdinalNumber-int-) | Mengatur nomor ordinal dari pola pengulangan bulanan. |
| [setMonthlyOrdinalRepetitions(int value)](#setMonthlyOrdinalRepetitions-int-) | Mengatur jumlah pengulangan untuk pola pengulangan bulanan saat menggunakan hari ordinal. |
| [setMonthlyRepetitions(int value)](#setMonthlyRepetitions-int-) | Mengatur jumlah pengulangan untuk pola pengulangan bulanan. |
| [setMonthlyUseOrdinalDay(boolean value)](#setMonthlyUseOrdinalDay-boolean-) | Mengatur nilai yang menunjukkan apakah akan menggunakan hari ordinal untuk pola pengulangan bulanan. |
| [setOccurrences(int value)](#setOccurrences-int-) | Mengatur jumlah kejadian dari tugas berulang. |
| [setRecurrencePattern(int value)](#setRecurrencePattern-int-) | Mengatur pola pengulangan dari tugas berulang. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | Mengatur tanggal mulai kejadian. |
| [setUseEndDate(boolean value)](#setUseEndDate-boolean-) | Mengatur nilai yang menunjukkan apakah akan menggunakan tanggal akhir atau jumlah kejadian untuk tugas berulang. |
| [setWeeklyDays(int value)](#setWeeklyDays-int-) | Mengatur kumpulan hari yang digunakan dalam pola pengulangan mingguan. |
| [setWeeklyRepetitions(int value)](#setWeeklyRepetitions-int-) | Mengatur jumlah pengulangan untuk pola pengulangan mingguan. |
| [setYearlyDate(Date value)](#setYearlyDate-java.util.Date-) | Mengatur tanggal untuk pola pengulangan tahunan. |
| [setYearlyOrdinalDay(int value)](#setYearlyOrdinalDay-int-) | Mengatur hari kerja dari pola pengulangan tahunan saat menggunakan hari ordinal. |
| [setYearlyOrdinalMonth(int value)](#setYearlyOrdinalMonth-int-) | Mengatur bulan dari pola pengulangan tahunan saat menggunakan hari ordinal. |
| [setYearlyOrdinalNumber(int value)](#setYearlyOrdinalNumber-int-) | Mengatur nomor ordinal dari pola pengulangan tahunan. |
| [setYearlyUseOrdinalDay(boolean value)](#setYearlyUseOrdinalDay-boolean-) | Mengatur nilai yang menunjukkan apakah akan menggunakan hari ordinal untuk pola pengulangan tahunan. |
### getDailyRepetitions() {#getDailyRepetitions--}
```
public final int getDailyRepetitions()
```


Mendapatkan jumlah pengulangan untuk pola berulang harian.

**Returns:**
int - jumlah pengulangan untuk pola berulang harian.
### getDailyUseWorkdays() {#getDailyUseWorkdays--}
```
public final boolean getDailyUseWorkdays()
```


Mendapatkan nilai yang menunjukkan apakah akan menggunakan hari kerja untuk pola berulang harian.

**Returns:**
boolean - nilai yang menunjukkan apakah akan menggunakan hari kerja untuk pola berulang harian.
### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Mendapatkan durasi untuk satu kejadian tugas berulang.

--------------------

instance dari `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskinfo\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskinfo\#setDuration-Duration-)) kelas.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the duration for one occurrence of the recurring task.
### getEndDate() {#getEndDate--}
```
public final Date getEndDate()
```


Mendapatkan tanggal berakhirnya kejadian.

**Returns:**
java.util.Date - tanggal untuk mengakhiri kejadian.
### getMonthlyDay() {#getMonthlyDay--}
```
public final int getMonthlyDay()
```


Mendapatkan jumlah hari dari pola berulang bulanan.

**Returns:**
int - jumlah hari dalam pola berulang bulanan.
### getMonthlyOrdinalDay() {#getMonthlyOrdinalDay--}
```
public final int getMonthlyOrdinalDay()
```


Mendapatkan hari dari pola berulang bulanan saat menggunakan hari ordinal.

--------------------

Bisa menjadi salah satu nilai dari enumerasi [DayOfWeek](../../com.aspose.tasks/dayofweek).

**Returns:**
int - hari dalam pola berulang bulanan ketika menggunakan hari ordinal.
### getMonthlyOrdinalNumber() {#getMonthlyOrdinalNumber--}
```
public final int getMonthlyOrdinalNumber()
```


Mendapatkan nomor ordinal dari pola berulang bulanan.

--------------------

Bisa menjadi salah satu nilai dari enumerasi [OrdinalNumber](../../com.aspose.tasks/ordinalnumber).

**Returns:**
int - nomor ordinal dari pola berulang bulanan.
### getMonthlyOrdinalRepetitions() {#getMonthlyOrdinalRepetitions--}
```
public final int getMonthlyOrdinalRepetitions()
```


Mendapatkan jumlah pengulangan untuk pola berulang bulanan saat menggunakan hari ordinal.

**Returns:**
int - jumlah pengulangan untuk pola berulang bulanan ketika menggunakan hari ordinal.
### getMonthlyRepetitions() {#getMonthlyRepetitions--}
```
public final int getMonthlyRepetitions()
```


Mendapatkan jumlah pengulangan untuk pola berulang bulanan.

**Returns:**
int - jumlah pengulangan untuk pola berulang bulanan.
### getMonthlyUseOrdinalDay() {#getMonthlyUseOrdinalDay--}
```
public final boolean getMonthlyUseOrdinalDay()
```


Mendapatkan nilai yang menunjukkan apakah akan menggunakan hari ordinal untuk pola berulang bulanan.

**Returns:**
boolean - nilai yang menunjukkan apakah akan menggunakan hari ordinal untuk pola berulang bulanan.
### getOccurrences() {#getOccurrences--}
```
public final int getOccurrences()
```


Mendapatkan jumlah kejadian tugas berulang.

**Returns:**
int - jumlah kejadian dari tugas berulang.
### getRecurrencePattern() {#getRecurrencePattern--}
```
public final int getRecurrencePattern()
```


Mendapatkan pola berulang dari tugas berulang.

--------------------

Bisa menjadi salah satu nilai dari enumerasi `RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskinfo\#getRecurrencePattern--)/[setRecurrencePattern(int)](../../com.aspose.tasks/recurringtaskinfo\#setRecurrencePattern-int-)).

**Returns:**
int - pola berulang dari tugas berulang.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


Mendapatkan tanggal mulai kejadian.

**Returns:**
java.util.Date - tanggal untuk memulai kejadian.
### getTask() {#getTask--}
```
public final Task getTask()
```


Mendapatkan tugas induk dari instance kelas [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo) ini.

**Returns:**
[Task](../../com.aspose.tasks/task) - the parent task of this instance of [RecurringTaskInfo](../../com.aspose.tasks/recurringtaskinfo) class.
### getUseEndDate() {#getUseEndDate--}
```
public final boolean getUseEndDate()
```


Mendapatkan nilai yang menunjukkan apakah akan menggunakan tanggal akhir atau jumlah kejadian untuk tugas berulang.

**Returns:**
boolean - nilai yang menunjukkan apakah akan menggunakan tanggal akhir atau jumlah kejadian untuk tugas berulang.
### getWeeklyDays() {#getWeeklyDays--}
```
public final int getWeeklyDays()
```


Mendapatkan kumpulan hari yang digunakan dalam pola berulang mingguan.

--------------------

**Returns:**
int - kumpulan hari yang digunakan dalam pola berulang mingguan.
### getWeeklyRepetitions() {#getWeeklyRepetitions--}
```
public final int getWeeklyRepetitions()
```


Mendapatkan jumlah pengulangan untuk pola berulang mingguan.

**Returns:**
int - jumlah pengulangan untuk pola berulang mingguan.
### getYearlyDate() {#getYearlyDate--}
```
public final Date getYearlyDate()
```


Mendapatkan tanggal untuk pola berulang tahunan.

**Returns:**
java.util.Date - tanggal untuk pola berulang tahunan.
### getYearlyOrdinalDay() {#getYearlyOrdinalDay--}
```
public final int getYearlyOrdinalDay()
```


Mendapatkan hari kerja dari pola pengulangan tahunan saat menggunakan hari ordinal.

--------------------

Bisa menjadi salah satu nilai dari enumerasi [DayOfWeek](../../com.aspose.tasks/dayofweek).

**Returns:**
int - hari kerja dalam pola berulang tahunan ketika menggunakan hari ordinal.
### getYearlyOrdinalMonth() {#getYearlyOrdinalMonth--}
```
public final int getYearlyOrdinalMonth()
```


Mendapatkan bulan dari pola pengulangan tahunan saat menggunakan hari ordinal.

--------------------

Bisa menjadi salah satu nilai dari enumerasi [Month](../../com.aspose.tasks/month).

**Returns:**
int - bulan dalam pola berulang tahunan ketika menggunakan hari ordinal.
### getYearlyOrdinalNumber() {#getYearlyOrdinalNumber--}
```
public final int getYearlyOrdinalNumber()
```


Mendapatkan nomor ordinal dari pola pengulangan tahunan.

--------------------

Bisa menjadi salah satu nilai dari enumerasi [OrdinalNumber](../../com.aspose.tasks/ordinalnumber).

**Returns:**
int - nomor ordinal dari pola berulang tahunan.
### getYearlyUseOrdinalDay() {#getYearlyUseOrdinalDay--}
```
public final boolean getYearlyUseOrdinalDay()
```


Mendapatkan nilai yang menunjukkan apakah akan menggunakan hari ordinal untuk pola pengulangan tahunan.

**Returns:**
boolean - nilai yang menunjukkan apakah akan menggunakan hari ordinal untuk pola berulang tahunan.
### setDailyRepetitions(int value) {#setDailyRepetitions-int-}
```
public final void setDailyRepetitions(int value)
```


Mengatur jumlah pengulangan untuk pola pengulangan harian.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | sejumlah pengulangan untuk pola berulang harian. |

### setDailyUseWorkdays(boolean value) {#setDailyUseWorkdays-boolean-}
```
public final void setDailyUseWorkdays(boolean value)
```


Mengatur nilai yang menunjukkan apakah akan menggunakan hari kerja untuk pola pengulangan harian.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah akan menggunakan hari kerja untuk pola berulang harian. |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Mengatur durasi untuk satu kejadian dari tugas berulang.

--------------------

instance dari `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskinfo\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskinfo\#setDuration-Duration-)) kelas.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | durasi untuk satu kejadian tugas berulang. |

### setEndDate(Date value) {#setEndDate-java.util.Date-}
```
public final void setEndDate(Date value)
```


Mengatur tanggal berakhirnya kejadian.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date | tanggal untuk mengakhiri kejadian. |

### setMonthlyDay(int value) {#setMonthlyDay-int-}
```
public final void setMonthlyDay(int value)
```


Mengatur jumlah hari dari pola pengulangan bulanan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | jumlah hari pada pola berulang bulanan. |

### setMonthlyOrdinalDay(int value) {#setMonthlyOrdinalDay-int-}
```
public final void setMonthlyOrdinalDay(int value)
```


Mengatur hari dari pola pengulangan bulanan saat menggunakan hari ordinal.

--------------------

Bisa menjadi salah satu nilai dari enumerasi [DayOfWeek](../../com.aspose.tasks/dayofweek).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | hari pada pola berulang bulanan ketika menggunakan hari ordinal. |

### setMonthlyOrdinalNumber(int value) {#setMonthlyOrdinalNumber-int-}
```
public final void setMonthlyOrdinalNumber(int value)
```


Mengatur nomor ordinal dari pola pengulangan bulanan.

--------------------

Bisa menjadi salah satu nilai dari enumerasi [OrdinalNumber](../../com.aspose.tasks/ordinalnumber).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | angka ordinal pada pola berulang bulanan. |

### setMonthlyOrdinalRepetitions(int value) {#setMonthlyOrdinalRepetitions-int-}
```
public final void setMonthlyOrdinalRepetitions(int value)
```


Mengatur jumlah pengulangan untuk pola pengulangan bulanan saat menggunakan hari ordinal.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | sejumlah pengulangan untuk pola berulang bulanan ketika menggunakan hari ordinal. |

### setMonthlyRepetitions(int value) {#setMonthlyRepetitions-int-}
```
public final void setMonthlyRepetitions(int value)
```


Mengatur jumlah pengulangan untuk pola pengulangan bulanan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | sejumlah pengulangan untuk pola berulang bulanan. |

### setMonthlyUseOrdinalDay(boolean value) {#setMonthlyUseOrdinalDay-boolean-}
```
public final void setMonthlyUseOrdinalDay(boolean value)
```


Mengatur nilai yang menunjukkan apakah akan menggunakan hari ordinal untuk pola pengulangan bulanan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah akan menggunakan hari ordinal untuk pola berulang bulanan. |

### setOccurrences(int value) {#setOccurrences-int-}
```
public final void setOccurrences(int value)
```


Mengatur jumlah kejadian dari tugas berulang.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | jumlah kejadian tugas berulang. |

### setRecurrencePattern(int value) {#setRecurrencePattern-int-}
```
public final void setRecurrencePattern(int value)
```


Mengatur pola pengulangan dari tugas berulang.

--------------------

Bisa menjadi salah satu nilai dari enumerasi `RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskinfo\#getRecurrencePattern--)/[setRecurrencePattern(int)](../../com.aspose.tasks/recurringtaskinfo\#setRecurrencePattern-int-)).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | pola berulang dari tugas berulang. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


Mengatur tanggal mulai kejadian.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date | tanggal untuk memulai kejadian. |

### setUseEndDate(boolean value) {#setUseEndDate-boolean-}
```
public final void setUseEndDate(boolean value)
```


Mengatur nilai yang menunjukkan apakah akan menggunakan tanggal akhir atau jumlah kejadian untuk tugas berulang.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah akan menggunakan tanggal akhir atau jumlah kejadian untuk tugas berulang. |

### setWeeklyDays(int value) {#setWeeklyDays-int-}
```
public final void setWeeklyDays(int value)
```


Mengatur kumpulan hari yang digunakan dalam pola pengulangan mingguan.

--------------------

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | koleksi hari yang digunakan dalam pola berulang mingguan. |

### setWeeklyRepetitions(int value) {#setWeeklyRepetitions-int-}
```
public final void setWeeklyRepetitions(int value)
```


Mengatur jumlah pengulangan untuk pola pengulangan mingguan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | sejumlah pengulangan untuk pola berulang mingguan. |

### setYearlyDate(Date value) {#setYearlyDate-java.util.Date-}
```
public final void setYearlyDate(Date value)
```


Mengatur tanggal untuk pola pengulangan tahunan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date | tanggal untuk pola berulang tahunan. |

### setYearlyOrdinalDay(int value) {#setYearlyOrdinalDay-int-}
```
public final void setYearlyOrdinalDay(int value)
```


Mengatur hari kerja dari pola pengulangan tahunan saat menggunakan hari ordinal.

--------------------

Bisa menjadi salah satu nilai dari enumerasi [DayOfWeek](../../com.aspose.tasks/dayofweek).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | hari kerja dalam pola berulang tahunan ketika menggunakan hari ordinal. |

### setYearlyOrdinalMonth(int value) {#setYearlyOrdinalMonth-int-}
```
public final void setYearlyOrdinalMonth(int value)
```


Mengatur bulan dari pola pengulangan tahunan saat menggunakan hari ordinal.

--------------------

Bisa menjadi salah satu nilai dari enumerasi [Month](../../com.aspose.tasks/month).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | bulan dalam pola berulang tahunan ketika menggunakan hari ordinal. |

### setYearlyOrdinalNumber(int value) {#setYearlyOrdinalNumber-int-}
```
public final void setYearlyOrdinalNumber(int value)
```


Mengatur nomor ordinal dari pola pengulangan tahunan.

--------------------

Bisa menjadi salah satu nilai dari enumerasi [OrdinalNumber](../../com.aspose.tasks/ordinalnumber).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | angka ordinal pada pola berulang tahunan. |

### setYearlyUseOrdinalDay(boolean value) {#setYearlyUseOrdinalDay-boolean-}
```
public final void setYearlyUseOrdinalDay(boolean value)
```


Mengatur nilai yang menunjukkan apakah akan menggunakan hari ordinal untuk pola pengulangan tahunan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah akan menggunakan hari ordinal untuk pola berulang tahunan. |

