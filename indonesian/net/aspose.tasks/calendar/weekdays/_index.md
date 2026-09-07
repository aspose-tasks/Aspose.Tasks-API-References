---
title: "Calendar.WeekDays"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Calendar. Mendapatkan WeekDaysCollection untuk kalender ini. Kumpulan hari kerja yang mendefinisikan kalender."
type: docs
weight: 120
url: /id/net/aspose.tasks/calendar/weekdays/
---
## Calendar.WeekDays property

Mendapatkan WeekDaysCollection untuk kalender ini. Kumpulan hari kerja yang mendefinisikan kalender.

```csharp
public WeekDayCollection WeekDays { get; }
```

## Contoh

Menampilkan cara mendefinisikan kalender baru, menambahkan hari kerja ke dalamnya, dan mendefinisikan waktu kerja untuk hari-hari.

```csharp
var project = new Project();

// Definisikan sebuah kalender
var calendar = project.Calendars.Add("Calendar1");

// Tambahkan hari kerja Senin hingga Kamis dengan jadwal default
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// Setel Jumat sebagai hari kerja pendek
var weekDay = new WeekDay(DayType.Friday);

// Mengatur waktu kerja. Hanya bagian waktu dari DateTime yang penting
var workingTime = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 16);
weekDay.WorkingTimes.Add(workingTime);
weekDay.WorkingTimes.Add(workingTime2);
weekDay.DayWorking = true;
calendar.WeekDays.Add(weekDay);

// bekerja dengan proyek...
```

### Lihat Juga

* class [WeekDayCollection](../../weekdaycollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


