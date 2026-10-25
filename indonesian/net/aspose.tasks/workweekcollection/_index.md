---
title: "Kelas WorkWeekCollection"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.WorkWeekCollection. Mewakili kumpulan objek WorkWeek"
type: docs
weight: 3650
url: /id/net/aspose.tasks/workweekcollection/
---
## WorkWeekCollection class

Mewakili kumpulan objek [`WorkWeek`](../workweek/).

```csharp
public class WorkWeekCollection : IList<WorkWeek>
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Count](../../aspose.tasks/workweekcollection/count/) { get; } | Mendapatkan jumlah objek yang terdapat dalam objek `WorkWeekCollection` ini. |
| [Item](../../aspose.tasks/workweekcollection/item/) { get; set; } | Mengembalikan elemen pada indeks yang ditentukan. |
| [ParentCalendar](../../aspose.tasks/workweekcollection/parentcalendar/) { get; } | Mendapatkan kalender induk. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Add](../../aspose.tasks/workweekcollection/add/)(WorkWeek) | Menambahkan instance WorkWeek ke objek koleksi ini. |
| [GetEnumerator](../../aspose.tasks/workweekcollection/getenumerator/)() | Mengembalikan enumerator untuk koleksi ini. |
| [ToList](../../aspose.tasks/workweekcollection/tolist/)() | Mengonversi objek WorkWeekCollection menjadi daftar objek [`WorkWeek`](../workweek/). |

## Contoh

Menampilkan cara membuat minggu kerja khusus untuk kalender.

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

Console.WriteLine("Work Weeks Count: " + calendar.WorkWeeks.Count);
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

* class [WorkWeek](../workweek/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


