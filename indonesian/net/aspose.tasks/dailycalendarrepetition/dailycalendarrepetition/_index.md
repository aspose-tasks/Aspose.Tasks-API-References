---
title: "DailyCalendarRepetition.DailyCalendarRepetition"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "DailyCalendarRepetition konstruktor. Menginisialisasi instance baru dari kelas DailyCalendarRepetition"
type: docs
weight: 10
url: /id/net/aspose.tasks/dailycalendarrepetition/dailycalendarrepetition/
---
## DailyCalendarRepetition constructor

Menginisialisasi instance baru dari kelas [`DailyCalendarRepetition`](../).

```csharp
public DailyCalendarRepetition()
```

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

* class [DailyCalendarRepetition](../)
* namespace [Aspose.Tasks](../../dailycalendarrepetition/)
* assembly [Aspose.Tasks](../../../)


