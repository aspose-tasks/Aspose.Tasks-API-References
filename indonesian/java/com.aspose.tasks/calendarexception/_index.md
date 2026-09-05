---
title: "CalendarException"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili periode waktu luar biasa dalam kalender."
type: docs
weight: 43
url: /id/java/com.aspose.tasks/calendarexception/
---

**Inheritance:**
java.lang.Object
```
public final class CalendarException
```

Mewakili periode waktu luar biasa dalam kalender.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [CalendarException()](#CalendarException--) | Menginisialisasi instance baru dari kelas [CalendarException](../../com.aspose.tasks/calendarexception). |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [checkException(Date dt)](#checkException-java.util.Date-) | Mengembalikan true jika instance yang ditentukan dari struct java.util.Date adalah hari pengecualian. |
| [delete()](#delete--) | Menghapus instance Exception dari objek CalendarExceptionCollection kalender induk. |
| [getDayWorking()](#getDayWorking--) | Mendapatkan nilai yang menunjukkan apakah tanggal atau tipe hari yang ditentukan merupakan hari kerja. |
| [getDaysOfWeek()](#getDaysOfWeek--) | Mendapatkan DayTypeCollection untuk objek ini. |
| [getEnteredByOccurrences()](#getEnteredByOccurrences--) | Mendapatkan nilai yang menunjukkan apakah rentang pengulangan didefinisikan dengan memasukkan jumlah kejadian. |
| [getExceptionDates()](#getExceptionDates--) | Mengembalikan tanggal-tanggal di mana pengecualian kalender berlaku. |
| [getFromDate()](#getFromDate--) | Mendapatkan awal waktu pengecualian. |
| [getMonth()](#getMonth--) | Mendapatkan bulan di mana pengulangan pengecualian dijadwalkan. |
| [getMonthDay()](#getMonthDay--) | Mendapatkan hari dalam bulan di mana pengulangan pengecualian dijadwalkan. |
| [getMonthItem()](#getMonthItem--) | Mendapatkan item bulan di mana pengulangan pengecualian dijadwalkan. |
| [getMonthPosition()](#getMonthPosition--) | Mendapatkan posisi item bulan dalam satu bulan. |
| [getName()](#getName--) | Mendapatkan nama pengecualian. |
| [getOccurrences()](#getOccurrences--) | Mendapatkan jumlah kejadian di mana pengecualian kalender berlaku. |
| [getParentCalendar()](#getParentCalendar--) | Mendapatkan kalender induk untuk objek ini. |
| [getPeriod()](#getPeriod--) | Mendapatkan periode pengulangan untuk pengecualian. |
| [getToDate()](#getToDate--) | Mendapatkan akhir waktu pengecualian. |
| [getType()](#getType--) | Mendapatkan tipe pengecualian. |
| [getWorkingTime()](#getWorkingTime--) | Mengembalikan waktu kerja untuk pengecualian kalender. |
| [getWorkingTimes()](#getWorkingTimes--) | Mendapatkan objek WorkingTimeCollection. |
| [setDayWorking(boolean value)](#setDayWorking-boolean-) | Mengatur nilai yang menunjukkan apakah tanggal atau tipe hari yang ditentukan merupakan hari kerja. |
| [setEnteredByOccurrences(boolean value)](#setEnteredByOccurrences-boolean-) | Mengatur nilai yang menunjukkan apakah rentang pengulangan didefinisikan dengan memasukkan jumlah kejadian. |
| [setFromDate(Date value)](#setFromDate-java.util.Date-) | Mengatur awal waktu pengecualian. |
| [setMonth(int value)](#setMonth-int-) | Mengatur bulan di mana pengulangan pengecualian dijadwalkan. |
| [setMonthDay(int value)](#setMonthDay-int-) | Mengatur hari dalam sebulan di mana pengulangan pengecualian dijadwalkan. |
| [setMonthItem(int value)](#setMonthItem-int-) | Mengatur item bulan untuk pengulangan pengecualian yang dijadwalkan. |
| [setMonthPosition(int value)](#setMonthPosition-int-) | Mengatur posisi item bulan dalam sebulan. |
| [setName(String value)](#setName-java.lang.String-) | Mengatur nama pengecualian. |
| [setOccurrences(int value)](#setOccurrences-int-) | Mengatur jumlah kejadian di mana pengecualian kalender berlaku. |
| [setPeriod(int value)](#setPeriod-int-) | Mengatur periode pengulangan untuk pengecualian. |
| [setToDate(Date value)](#setToDate-java.util.Date-) | Mengatur akhir waktu pengecualian. |
| [setType(int value)](#setType-int-) | Mengatur tipe pengecualian. |
| [setWorkingTimes(WorkingTimeCollection value)](#setWorkingTimes-com.aspose.tasks.WorkingTimeCollection-) | Mengatur objek WorkingTimeCollection. |
### CalendarException() {#CalendarException--}
```
public CalendarException()
```


Menginisialisasi instance baru dari kelas [CalendarException](../../com.aspose.tasks/calendarexception).

### checkException(Date dt) {#checkException-java.util.Date-}
```
public final boolean checkException(Date dt)
```


Mengembalikan true jika instance yang ditentukan dari struct java.util.Date adalah hari pengecualian.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| dt | java.util.Date | instance yang ditentukan dari struct java.util.Date. |

**Returns:**
boolean - Mengembalikan true jika nilai java.util.Date adalah hari pengecualian; jika tidak, false.
### delete() {#delete--}
```
public final void delete()
```


Menghapus instance Exception dari objek CalendarExceptionCollection kalender induk.

### getDayWorking() {#getDayWorking--}
```
public final boolean getDayWorking()
```


Mendapatkan nilai yang menunjukkan apakah tanggal atau tipe hari yang ditentukan merupakan hari kerja.

**Returns:**
boolean - nilai yang menunjukkan apakah tanggal atau tipe hari yang ditentukan sedang bekerja.
### getDaysOfWeek() {#getDaysOfWeek--}
```
public final DayTypeCollection getDaysOfWeek()
```


Mendapatkan DayTypeCollection untuk objek ini. Hari-hari dalam seminggu di mana pengecualian berlaku.

**Returns:**
[DayTypeCollection](../../com.aspose.tasks/daytypecollection) - the DayTypeCollection for this object.
### getEnteredByOccurrences() {#getEnteredByOccurrences--}
```
public final boolean getEnteredByOccurrences()
```


Mendapatkan nilai yang menunjukkan apakah rentang pengulangan didefinisikan dengan memasukkan jumlah kejadian. False menunjukkan bahwa rentang pengulangan didefinisikan dengan memasukkan tanggal selesai.

**Returns:**
boolean - nilai yang menunjukkan apakah rentang pengulangan didefinisikan dengan memasukkan jumlah kejadian.
### getExceptionDates() {#getExceptionDates--}
```
public final Iterable<Date> getExceptionDates()
```


Mengembalikan tanggal-tanggal di mana pengecualian kalender berlaku.

**Returns:**
java.lang.Iterable&lt;java.util.Date&gt; - tanggal di mana pengecualian kalender berlaku.
### getFromDate() {#getFromDate--}
```
public final Date getFromDate()
```


Mendapatkan awal waktu pengecualian.

**Returns:**
java.util.Date - awal waktu pengecualian.
### getMonth() {#getMonth--}
```
public final int getMonth()
```


Mendapatkan bulan di mana pengulangan pengecualian dijadwalkan.

**Returns:**
int - bulan di mana pengulangan pengecualian dijadwalkan.
### getMonthDay() {#getMonthDay--}
```
public final int getMonthDay()
```


Mendapatkan hari dalam bulan di mana pengulangan pengecualian dijadwalkan.

**Returns:**
int - hari dalam sebulan di mana pengulangan pengecualian dijadwalkan.
### getMonthItem() {#getMonthItem--}
```
public final int getMonthItem()
```


Mendapatkan item bulan di mana pengulangan pengecualian dijadwalkan.

**Returns:**
int - item bulan untuk pengulangan pengecualian yang dijadwalkan.
### getMonthPosition() {#getMonthPosition--}
```
public final int getMonthPosition()
```


Mendapatkan posisi item bulan dalam satu bulan.

**Returns:**
int - posisi item bulan dalam sebulan.
### getName() {#getName--}
```
public final String getName()
```


Mendapatkan nama pengecualian.

**Returns:**
java.lang.String - nama pengecualian.
### getOccurrences() {#getOccurrences--}
```
public final int getOccurrences()
```


Mendapatkan jumlah kejadian di mana pengecualian kalender berlaku.

**Returns:**
int - jumlah kejadian di mana pengecualian kalender berlaku.
### getParentCalendar() {#getParentCalendar--}
```
public final Calendar getParentCalendar()
```


Mendapatkan kalender induk untuk objek ini.

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - the parent calendar for this object.
### getPeriod() {#getPeriod--}
```
public final int getPeriod()
```


Mendapatkan periode pengulangan untuk pengecualian.

**Returns:**
int - periode pengulangan untuk pengecualian.
### getToDate() {#getToDate--}
```
public final Date getToDate()
```


Mendapatkan akhir waktu pengecualian.

**Returns:**
java.util.Date - akhir waktu pengecualian.
### getType() {#getType--}
```
public final int getType()
```


Mendapatkan tipe pengecualian.

**Returns:**
int - tipe pengecualian.
### getWorkingTime() {#getWorkingTime--}
```
public final double getWorkingTime()
```


Mengembalikan waktu kerja untuk pengecualian kalender.

**Returns:**
double - Mengembalikan waktu kerja untuk pengecualian kalender ini.
### getWorkingTimes() {#getWorkingTimes--}
```
public final WorkingTimeCollection getWorkingTimes()
```


Mendapatkan objek WorkingTimeCollection. Koleksi waktu kerja yang mendefinisikan waktu kerja pada hari kerja.

--------------------

Setidaknya satu waktu kerja harus ada, dan tidak boleh lebih dari lima.

**Returns:**
[WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) - the WorkingTimeCollection object.
### setDayWorking(boolean value) {#setDayWorking-boolean-}
```
public final void setDayWorking(boolean value)
```


Mengatur nilai yang menunjukkan apakah tanggal atau tipe hari yang ditentukan merupakan hari kerja.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah tanggal atau tipe hari yang ditentukan sedang bekerja. |

### setEnteredByOccurrences(boolean value) {#setEnteredByOccurrences-boolean-}
```
public final void setEnteredByOccurrences(boolean value)
```


Mengatur nilai yang menunjukkan apakah rentang pengulangan didefinisikan dengan memasukkan jumlah kejadian. False menunjukkan bahwa rentang pengulangan didefinisikan dengan memasukkan tanggal selesai.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah rentang pengulangan didefinisikan dengan memasukkan jumlah kejadian. |

### setFromDate(Date value) {#setFromDate-java.util.Date-}
```
public final void setFromDate(Date value)
```


Mengatur awal waktu pengecualian.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date | awal waktu pengecualian. |

### setMonth(int value) {#setMonth-int-}
```
public final void setMonth(int value)
```


Mengatur bulan di mana pengulangan pengecualian dijadwalkan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | bulan di mana pengulangan pengecualian dijadwalkan. |

### setMonthDay(int value) {#setMonthDay-int-}
```
public final void setMonthDay(int value)
```


Mengatur hari dalam sebulan di mana pengulangan pengecualian dijadwalkan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | hari dalam bulan di mana pengulangan pengecualian dijadwalkan. |

### setMonthItem(int value) {#setMonthItem-int-}
```
public final void setMonthItem(int value)
```


Mengatur item bulan untuk pengulangan pengecualian yang dijadwalkan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | item bulan untuk pengulangan pengecualian yang dijadwalkan. |

### setMonthPosition(int value) {#setMonthPosition-int-}
```
public final void setMonthPosition(int value)
```


Mengatur posisi item bulan dalam sebulan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | posisi item bulan dalam satu bulan. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Mengatur nama pengecualian.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | nama pengecualian. |

### setOccurrences(int value) {#setOccurrences-int-}
```
public final void setOccurrences(int value)
```


Mengatur jumlah kejadian di mana pengecualian kalender berlaku.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | jumlah kejadian di mana pengecualian kalender berlaku. |

### setPeriod(int value) {#setPeriod-int-}
```
public final void setPeriod(int value)
```


Mengatur periode pengulangan untuk pengecualian.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | periode pengulangan untuk pengecualian. |

### setToDate(Date value) {#setToDate-java.util.Date-}
```
public final void setToDate(Date value)
```


Mengatur akhir waktu pengecualian.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date | akhir waktu pengecualian. |

### setType(int value) {#setType-int-}
```
public final void setType(int value)
```


Mengatur tipe pengecualian.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | tipe pengecualian. |

### setWorkingTimes(WorkingTimeCollection value) {#setWorkingTimes-com.aspose.tasks.WorkingTimeCollection-}
```
public final void setWorkingTimes(WorkingTimeCollection value)
```


Mengatur objek WorkingTimeCollection. Koleksi waktu kerja yang mendefinisikan waktu kerja pada hari kerja.

--------------------

Setidaknya satu waktu kerja harus ada, dan tidak boleh lebih dari lima.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [WorkingTimeCollection](../../com.aspose.tasks/workingtimecollection) | objek WorkingTimeCollection. |

