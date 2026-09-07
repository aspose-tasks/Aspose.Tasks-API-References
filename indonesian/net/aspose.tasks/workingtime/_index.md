---
title: "Kelas WorkingTime"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.WorkingTime. Mewakili waktu kerja selama hari kerja."
type: docs
weight: 3660
url: /id/net/aspose.tasks/workingtime/
---
## WorkingTime class

Mewakili waktu kerja selama hari kerja.

```csharp
public class WorkingTime
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [WorkingTime](workingtime/#constructor_1)(DateTime, DateTime) | Menginisialisasi instance baru kelas `WorkingTime` dengan interval yang memiliki waktu mulai dan selesai yang ditentukan. |
| [WorkingTime](workingtime/#constructor)(int, int) | Menginisialisasi instance baru kelas `WorkingTime` dengan item interval yang memiliki waktu mulai dan selesai yang ditentukan. |
| [WorkingTime](workingtime/#constructor_2)(TimeSpan, TimeSpan) | Menginisialisasi instance baru kelas `WorkingTime` dengan item interval yang memiliki waktu mulai dan selesai yang ditentukan. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [From](../../aspose.tasks/workingtime/from/) { get; } | Mendapatkan awal waktu kerja. |
| [To](../../aspose.tasks/workingtime/to/) { get; } | Mendapatkan akhir waktu kerja. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| override [Equals](../../aspose.tasks/workingtime/equals/)(object) | Memeriksa bahwa objek-objek tersebut sama. |
| override [GetHashCode](../../aspose.tasks/workingtime/gethashcode/)() | Mengembalikan nilai kode hash untuk instance kelas `WorkingTime`. |

## Contoh

Menampilkan cara bekerja dengan informasi waktu kerja.

```csharp
public void WorkWithWorkingTime()
{
    var project = new Project();
    var calendar = CreateCalendar(project);
    project.Set(Prj.Calendar, calendar);

    Console.WriteLine("Work Week Number: " + calendar.WeekDays.Count);

    // Data ini semua tentang tombol "Details." Anda dapat mengatur waktu kerja khusus untuk Hari Kerja khusus atau bahkan menjadikannya tidak bekerja.
    List<WeekDay> weekDays = calendar.WeekDays.ToList();
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
}

public static Calendar CreateCalendar(Project project)
{
    var calendar = project.Calendars.Add("MyCalendar", project.Calendars.GetByName("Standard"));
    var workingTimes = new List<WorkingTime>
                           {
                               new WorkingTime(new DateTime(1, 1, 1, 9, 0, 0), new DateTime(1, 1, 1, 12, 0, 0)),
                               new WorkingTime(new DateTime(1, 1, 1, 13, 0, 0), new DateTime(1, 1, 1, 18, 0, 0))
                           };

    calendar.WeekDays.Add(new WeekDay(DayType.Monday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Tuesday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Wednesday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Thursday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Friday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
    calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

    return calendar;
}
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


