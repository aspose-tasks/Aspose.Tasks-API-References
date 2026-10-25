---
title: "Enum MonthItemType"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Aspose.Tasks.MonthItemType enum. Menentukan item bulan untuk mana pengulangan pengecualian dijadwalkan."
type: docs
weight: 1050
url: /id/net/aspose.tasks/monthitemtype/
---
## MonthItemType enumeration

Menentukan item bulan untuk mana pengulangan pengecualian dijadwalkan.

```csharp
public enum MonthItemType
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| Undefined | `-1` | Menunjukkan tipe item bulan Undefined. |
| Day | `0` | Menunjukkan tipe item bulan Day. |
| Weekday | `1` | Menunjukkan tipe item bulan Weekday. |
| WeekendDay | `2` | Menunjukkan tipe item bulan WeekendDay. |
| Sunday | `3` | Menunjukkan tipe item bulan Sunday. |
| Monday | `4` | Menunjukkan tipe item bulan Monday. |
| Tuesday | `5` | Menunjukkan tipe item bulan Tuesday. |
| Wednesday | `6` | Menunjukkan tipe item bulan Wednesday. |
| Thursday | `7` | Menunjukkan tipe item bulan Thursday. |
| Friday | `8` | Menunjukkan tipe item bulan Friday. |
| Saturday | `9` | Menunjukkan tipe item bulan Saturday. |

## Contoh

Menampilkan cara mendefinisikan pengecualian kalender berdasarkan hari bulan.

```csharp
var project = new Project(DataDir + "project_test.mpp");

// Buat kalender
var calendar = project.Calendars.Add("Calendar1");

// Buat pengecualian kalender untuk setiap Jumat
var exception = new CalendarException();
exception.Type = CalendarExceptionType.MonthlyByDay;
exception.FromDate = new DateTime(2010, 1, 1);
exception.ToDate = new DateTime(2020, 12, 31);
exception.Month = Month.December;
exception.MonthDay = 1;
exception.MonthItem = MonthItemType.Undefined;
exception.MonthPosition = MonthPosition.Last;
exception.Period = 5;

// Periksa bahwa Jumat aa adalah pengecualian
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2012, 12, 1)));

// tambahkan pengecualian ke kalender
calendar.Exceptions.Add(exception);
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


