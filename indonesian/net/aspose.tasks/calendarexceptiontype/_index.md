---
title: "Enum CalendarExceptionType"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.CalendarExceptionType enum. Menentukan tipe pengecualian kalender"
type: docs
weight: 270
url: /id/net/aspose.tasks/calendarexceptiontype/
---
## CalendarExceptionType enumeration

Menentukan tipe pengecualian kalender.

```csharp
public enum CalendarExceptionType
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| Daily | `0` | Menunjukkan tipe pengecualian Harian. |
| YearlyByDay | `1` | Menunjukkan tipe pengecualian Tahunan berdasarkan hari dalam bulan. |
| YearlyByPosition | `2` | Menunjukkan tipe pengecualian Tahunan berdasarkan posisi. |
| MonthlyByDay | `3` | Menunjukkan tipe pengecualian Bulanan berdasarkan hari dalam bulan. |
| MonthlyByPosition | `4` | Menunjukkan tipe pengecualian Bulanan berdasarkan posisi. |
| Weekly | `5` | Menunjukkan tipe pengecualian mingguan. |
| ByDayCount | `6` | Menunjukkan tipe pengecualian berdasarkan hitungan hari. |
| ByWeekDayCount | `7` | Menunjukkan tipe pengecualian berdasarkan hitungan hari kerja. |
| NoExceptionType | `8` | Menunjukkan tidak ada tipe pengecualian. |

## Contoh

Menampilkan cara mendefinisikan pengecualian kalender berdasarkan kejadian.

```csharp
var project = new Project();

// Definisikan sebuah kalender
var calendar = project.Calendars.Add("Calendar1");

// Definisikan pengecualian dan tentukan kejadian
var exception = new CalendarException();
exception.EnteredByOccurrences = true;
exception.Occurrences = 5;
exception.Type = CalendarExceptionType.YearlyByDay;
exception.MonthDay = 22;
exception.Month = Month.April;

// Tambahkan pengecualian ke kalender
calendar.Exceptions.Add(exception);
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


