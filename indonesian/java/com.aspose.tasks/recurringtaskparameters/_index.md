---
title: "RecurringTaskParameters"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili sekumpulan parameter yang digunakan untuk membuat tugas berulang dalam sebuah proyek."
type: docs
weight: 245
url: /id/java/com.aspose.tasks/recurringtaskparameters/
---

**Inheritance:**
java.lang.Object
```
public class RecurringTaskParameters
```

Mewakili sekumpulan parameter yang digunakan untuk membuat tugas berulang dalam sebuah proyek.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [RecurringTaskParameters()](#RecurringTaskParameters--) | Menginisialisasi instance baru dari kelas [RecurringTaskParameters](../../com.aspose/tasks/recurringtaskparameters). |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getDuration()](#getDuration--) | Mendapatkan durasi untuk satu kejadian tugas berulang. |
| [getIgnoreResourceCalendar()](#getIgnoreResourceCalendar--) | Mendapatkan nilai yang menunjukkan apakah akan menjadwalkan tugas berulang meskipun tidak terjadi ketika ada sumber daya yang tersedia untuk mengerjakannya. |
| [getRecurrencePattern()](#getRecurrencePattern--) | Mendapatkan pola pengulangan dari tugas berulang. |
| [getTaskName()](#getTaskName--) | Mendapatkan nama tugas berulang. |
| [setCalendar(Project project, String calendarName)](#setCalendar-com.aspose.tasks.Project-java.lang.String-) | Atur kalender untuk tugas berulang. |
| [setDuration(Duration value)](#setDuration-com.aspose.tasks.Duration-) | Mengatur durasi untuk satu kejadian dari tugas berulang. |
| [setIgnoreResourceCalendar(boolean value)](#setIgnoreResourceCalendar-boolean-) | Mengatur nilai yang menunjukkan apakah akan menjadwalkan tugas berulang meskipun tidak terjadi ketika ada sumber daya yang tersedia untuk mengerjakannya. |
| [setRecurrencePattern(RecurrencePatternBase value)](#setRecurrencePattern-com.aspose.tasks.RecurrencePatternBase-) | Mengatur pola pengulangan dari tugas berulang. |
| [setTaskName(String value)](#setTaskName-java.lang.String-) | Mengatur nama tugas berulang. |
### RecurringTaskParameters() {#RecurringTaskParameters--}
```
public RecurringTaskParameters()
```


Menginisialisasi instance baru dari kelas [RecurringTaskParameters](../../com.aspose/tasks/recurringtaskparameters).

### getDuration() {#getDuration--}
```
public final Duration getDuration()
```


Mendapatkan durasi untuk satu kejadian tugas berulang.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - The instance of `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskparameters\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskparameters\#setDuration-Duration-)) class.
### getIgnoreResourceCalendar() {#getIgnoreResourceCalendar--}
```
public final boolean getIgnoreResourceCalendar()
```


Mendapatkan nilai yang menunjukkan apakah akan menjadwalkan tugas berulang meskipun tidak terjadi ketika ada sumber daya yang tersedia untuk mengerjakannya.

**Returns:**
boolean - nilai yang menunjukkan apakah menjadwalkan tugas berulang bahkan jika tidak terjadi ketika tidak ada sumber daya yang tersedia untuk mengerjakannya.
### getRecurrencePattern() {#getRecurrencePattern--}
```
public final RecurrencePatternBase getRecurrencePattern()
```


Mendapatkan pola pengulangan dari tugas berulang.

--------------------

Dapat menjadi salah satu nilai dari enumerasi `RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskparameters\#getRecurrencePattern--)/[setRecurrencePattern(RecurrencePatternBase)](../../com.aspose.tasks/recurringtaskparameters\#setRecurrencePattern-RecurrencePatternBase-)).

**Returns:**
[RecurrencePatternBase](../../com.aspose.tasks/recurrencepatternbase) - the recurrence pattern of the recurring task.
### getTaskName() {#getTaskName--}
```
public final String getTaskName()
```


Mendapatkan nama tugas berulang.

**Returns:**
java.lang.String - nama tugas berulang.
### setCalendar(Project project, String calendarName) {#setCalendar-com.aspose.tasks.Project-java.lang.String-}
```
public final void setCalendar(Project project, String calendarName)
```


Atur kalender untuk tugas berulang. Kalender dipilih dari koleksi kalender proyek.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Proyek dengan koleksi kalender. |
| calendarName | java.lang.String | Nama kalender. |

### setDuration(Duration value) {#setDuration-com.aspose.tasks.Duration-}
```
public final void setDuration(Duration value)
```


Mengatur durasi untuk satu kejadian dari tugas berulang.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [Duration](../../com.aspose.tasks/duration) | Instansi dari kelas `Duration`([getDuration()](../../com.aspose.tasks/recurringtaskparameters\#getDuration--)/[setDuration(Duration)](../../com.aspose.tasks/recurringtaskparameters\#setDuration-Duration-)). |

### setIgnoreResourceCalendar(boolean value) {#setIgnoreResourceCalendar-boolean-}
```
public final void setIgnoreResourceCalendar(boolean value)
```


Mengatur nilai yang menunjukkan apakah akan menjadwalkan tugas berulang meskipun tidak terjadi ketika ada sumber daya yang tersedia untuk mengerjakannya.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | nilai yang menunjukkan apakah menjadwalkan tugas berulang meskipun tidak terjadi ketika tidak ada sumber daya yang tersedia untuk mengerjakannya. |

### setRecurrencePattern(RecurrencePatternBase value) {#setRecurrencePattern-com.aspose.tasks.RecurrencePatternBase-}
```
public final void setRecurrencePattern(RecurrencePatternBase value)
```


Mengatur pola pengulangan dari tugas berulang.

--------------------

Dapat menjadi salah satu nilai dari enumerasi `RecurrencePattern`([getRecurrencePattern()](../../com.aspose.tasks/recurringtaskparameters\#getRecurrencePattern--)/[setRecurrencePattern(RecurrencePatternBase)](../../com.aspose.tasks/recurringtaskparameters\#setRecurrencePattern-RecurrencePatternBase-)).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| value | [RecurrencePatternBase](../../com.aspose.tasks/recurrencepatternbase) | pola pengulangan dari tugas berulang. |

### setTaskName(String value) {#setTaskName-java.lang.String-}
```
public final void setTaskName(String value)
```


Mengatur nama tugas berulang.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | nama tugas berulang. |

