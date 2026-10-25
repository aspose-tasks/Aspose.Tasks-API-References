---
title: "Kelas DailyCalendarRepetition"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.DailyCalendarRepetition. Mewakili kelas untuk pengulangan dalam pola berulang harian berdasarkan hari kalender"
type: docs
weight: 390
url: /id/net/aspose.tasks/dailycalendarrepetition/
---
## DailyCalendarRepetition class

Mewakili kelas untuk pengulangan dalam pola berulang harian berdasarkan hari kalender.

```csharp
public class DailyCalendarRepetition : DailyRepetitionBase
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [DailyCalendarRepetition](dailycalendarrepetition/)() | Menginisialisasi instansi baru dari kelas `DailyCalendarRepetition`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [RepetitionInterval](../../aspose.tasks/dailyrepetitionbase/repetitioninterval/) { get; set; } | Mendapatkan atau mengatur jumlah hari yang mewakili interval dalam hari antara kejadian. |

## Contoh

Menampilkan cara bekerja dengan pengulangan pola kerja harian dan '24 Jam' saat membuat tugas berulang.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var calendar = project.Calendars.Add("24 Hours");
Calendar.Make24HourCalendar(calendar);
var parameters = new RecurringTaskParameters
{
    TaskName = "t1",
    Duration = project.GetDuration(1, TimeUnitType.Day),
    RecurrencePattern = new DailyRecurrencePattern
    {
        Repetition = new DailyCalendarRepetition { RepetitionInterval = 1 },
        RecurrenceRange = new EndByRecurrenceRange
        {
            Start = new DateTime(2018, 7, 2, 0, 0, 0),
            Finish = new DateTime(2018, 7, 8, 16, 0, 0)
        }
    }
};
parameters.SetCalendar(project, "24 Hours");
project.RootTask.Children.Add(parameters);

// lanjutkan bekerja dengan proyek...
project.Save(OutDir + "CanAddRecurringTask_Days_CalendarDays_24h_Test_out.mpp", SaveFileFormat.Mpp);
```

### Lihat Juga

* class [DailyRepetitionBase](../dailyrepetitionbase/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


