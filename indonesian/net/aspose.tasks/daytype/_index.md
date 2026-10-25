---
title: "Enum DayType"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Enum Aspose.Tasks.DayType. Menentukan hari dalam seminggu"
type: docs
weight: 450
url: /id/net/aspose.tasks/daytype/
---
## DayType enumeration

Menentukan hari dalam seminggu.

```csharp
public enum DayType
```

### Nilai

| Nama | Nilai | Deskripsi |
| --- | --- | --- |
| Exception | `0` | Menunjukkan tipe hari Pengecualian. |
| Sunday | `1` | Menunjukkan tipe hari Minggu. |
| Monday | `2` | Menunjukkan tipe hari Senin. |
| Tuesday | `3` | Menunjukkan tipe hari Selasa. |
| Wednesday | `4` | Menunjukkan tipe hari Rabu. |
| Thursday | `5` | Menunjukkan tipe hari Kamis. |
| Friday | `6` | Menunjukkan tipe hari Jumat. |
| Saturday | `7` | Menunjukkan tipe hari Sabtu. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


