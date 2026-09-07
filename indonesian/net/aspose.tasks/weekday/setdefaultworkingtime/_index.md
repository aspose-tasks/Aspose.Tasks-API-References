---
title: "WeekDay.SetDefaultWorkingTime"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "WeekDay metode. Mengatur periode waktu default untuk hari minggu yang ditentukan"
type: docs
weight: 130
url: /id/net/aspose.tasks/weekday/setdefaultworkingtime/
---
## WeekDay.SetDefaultWorkingTime method

Mengatur periode waktu default untuk hari kerja yang ditentukan.

```csharp
public static void SetDefaultWorkingTime(WeekDay day)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| hari | WeekDay | Hari minggu untuk mengatur hari kerja default. |

## Contoh

Menampilkan cara mengatur waktu kerja default untuk satu hari.

```csharp
var project = new Project();

// Definisikan sebuah kalender
var calendar = project.Calendars.Add("Calendar1");
calendar.WeekDays.Clear();

// Tambahkan hari kerja Senin hingga Kamis dengan jadwal default
var monday = new WeekDay(DayType.Monday);
WeekDay.SetDefaultWorkingTime(monday);
calendar.WeekDays.Add(monday);
var tuesday = new WeekDay(DayType.Tuesday);
WeekDay.SetDefaultWorkingTime(tuesday);
calendar.WeekDays.Add(tuesday);
var wednesday = new WeekDay(DayType.Wednesday);
WeekDay.SetDefaultWorkingTime(wednesday);
calendar.WeekDays.Add(wednesday);
var thursday = new WeekDay(DayType.Thursday);
WeekDay.SetDefaultWorkingTime(thursday);
calendar.WeekDays.Add(thursday);
var friday = new WeekDay(DayType.Friday);
WeekDay.SetDefaultWorkingTime(friday);
calendar.WeekDays.Add(friday);

var saturday = new WeekDay(DayType.Saturday);
saturday.DayWorking = false;
calendar.WeekDays.Add(saturday);
var sunday = new WeekDay(DayType.Sunday);
sunday.DayWorking = false;
calendar.WeekDays.Add(sunday);

// mari cetak semua waktu kerja
foreach (var day in calendar.WeekDays)
{
    Console.WriteLine("Day Type: " + day.DayType); 
    Console.WriteLine("Is working day: " + day.DayWorking); 
    Console.WriteLine("Working Time (Hours): " + day.GetWorkingTime().TotalHours);
    Console.WriteLine();
}
```

### Lihat Juga

* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)


