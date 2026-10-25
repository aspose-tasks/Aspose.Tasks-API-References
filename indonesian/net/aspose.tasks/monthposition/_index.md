---
title: "Enum MonthPosition"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Enum Aspose.Tasks.MonthPosition. Menentukan posisi item bulan dalam sebulan."
type: docs
weight: 1070
url: /id/net/aspose.tasks/monthposition/
---
## MonthPosition enumeration

Menentukan posisi item bulan dalam satu bulan.

```csharp
public enum MonthPosition
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| Undefined | `-1` | Menunjukkan posisi bulan yang tidak terdefinisi. |
| First | `0` | Menunjukkan posisi bulan pertama. |
| Second | `1` | Menunjukkan posisi bulan kedua. |
| Third | `2` | Menunjukkan posisi bulan ketiga. |
| Fourth | `3` | Menunjukkan posisi bulan keempat. |
| Last | `4` | Menunjukkan posisi bulan terakhir. |

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


