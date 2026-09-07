---
title: "WeekDay.CreateDefaultWorkingDay"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode WeekDay. Membuat hari kerja default"
type: docs
weight: 20
url: /id/net/aspose.tasks/weekday/createdefaultworkingday/
---
## WeekDay.CreateDefaultWorkingDay method

Membuat hari kerja default.

```csharp
public static WeekDay CreateDefaultWorkingDay(DayType dayType)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| dayType | DayType | Tipe hari untuk membuat hari kerja default. |

### Nilai Kembali

Hari kerja default dengan jam kerja 8-12 dan 13-17.

## Contoh

Menampilkan cara membuat kalender baru dengan mendefinisikan hari kerja.

```csharp
var project = new Project();

// Definisikan sebuah kalender
var calendar = project.Calendars.Add("Calendar1");

// Tambahkan hari kerja Senin hingga Kamis dengan jadwal default
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(new WeekDay(DayType.Tuesday, new WorkingTime(9, 11), new WorkingTime(12, 18)));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));

var exceptionDay = WeekDay.CreateDefaultWorkingDay(DayType.Exception);
exceptionDay.FromDate = new DateTime(2020, 4, 27, 0, 0, 0);
exceptionDay.ToDate = new DateTime(2020, 4, 30, 0, 0, 0);
exceptionDay.DayWorking = false;
calendar.WeekDays.Add(exceptionDay);

// periksa tanggal mulai dan selesai hari pengecualian
Console.WriteLine("The from date is: " + exceptionDay.FromDate);
Console.WriteLine("The to date is: " + exceptionDay.ToDate);
Console.WriteLine();

calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// Setel Jumat sebagai hari kerja pendek

// Mengatur waktu kerja. 
var workingTimes = new List<WorkingTime> { new WorkingTime(9, 12), new WorkingTime(13, 16) };

// ada cara untuk mengonversi <see cref="DayOfWeek" /> menjadi <see cref="Aspose.Tasks.DayType" />.
var dayType = WeekDay.CastToDayType(DayOfWeek.Friday);

var weekDay = new WeekDay(dayType, workingTimes);
weekDay.DayWorking = true;
Console.WriteLine("The day type is: " + weekDay.DayType);
Console.WriteLine("The from date is: " + weekDay.FromDate);
Console.WriteLine("The to date is: " + weekDay.ToDate);

calendar.WeekDays.Add(weekDay);

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

* enum [DayType](../../daytype/)
* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)


