---
title: "Kelas WorkWeek"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.WorkWeek. Mewakili kelas WorkWeek"
type: docs
weight: 3640
url: /id/net/aspose.tasks/workweek/
---
## WorkWeek class

Mewakili kelas WorkWeek

```csharp
public class WorkWeek
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [WorkWeek](workweek/)() | Menginisialisasi sebuah instance baru dari kelas `WorkWeek`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [FromDate](../../aspose.tasks/workweek/fromdate/) { get; set; } | Mendapatkan atau mengatur DateTime mulai minggu kerja |
| [Name](../../aspose.tasks/workweek/name/) { get; set; } | Mendapatkan atau mengatur Name minggu kerja |
| [ToDate](../../aspose.tasks/workweek/todate/) { get; set; } | Mendapatkan atau mengatur Finish DateTime minggu kerja |
| [WeekDays](../../aspose.tasks/workweek/weekdays/) { get; } | Mendapatkan hari-hari dalam minggu. |

## Contoh

Menampilkan cara membaca informasi minggu kerja dari proyek.

```csharp
var project = new Project();
var calendar = project.Calendars.Add("Standard");
Calendar.MakeStandardCalendar(calendar);

var item = new WorkWeek();
item.Name = "My Work Week";
item.FromDate = new DateTime(2020, 4, 13, 8, 0, 0);
item.ToDate = new DateTime(2020, 4, 17, 17, 0, 0);
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));
item.WeekDays.Add(new WeekDay(DayType.Saturday));
item.WeekDays.Add(new WeekDay(DayType.Sunday));
calendar.WorkWeeks.Add(item);

Console.WriteLine("Work Week Number: " + calendar.WeekDays.Count);
foreach (var workWeek in calendar.WorkWeeks)
{
    // Tampilkan nama minggu kerja, nama kalender induk, tanggal mulai, dan tanggal akhir
    Console.WriteLine("Name: " + workWeek.Name);
    Console.WriteLine("Parent calendar name: " + calendar.Name);
    Console.WriteLine("From Date: " + workWeek.FromDate);
    Console.WriteLine("To Date: " + workWeek.ToDate);
    Console.WriteLine();

    // Data ini semua tentang tombol "Details." Anda dapat mengatur waktu kerja khusus untuk Hari Kerja khusus atau bahkan menjadikannya tidak bekerja.
    List<WeekDay> weekDays = workWeek.WeekDays.ToList();
    foreach (var day in weekDays)
    {
        Console.WriteLine(day.DayType.ToString());

        // Anda dapat menelusuri lebih lanjut melalui waktu kerja dan menampilkannya.
        foreach (var workingTime in day.WorkingTimes)
        {
            Console.WriteLine(workingTime.From);
            Console.WriteLine(workingTime.To);
        }
    }

    Console.WriteLine();
}
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


