---
title: "WorkingTime.WorkingTime"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "konstruktor WorkingTime. Menginisialisasi instance baru dari kelas WorkingTime dengan interval yang memiliki waktu mulai dan selesai yang ditentukan."
type: docs
weight: 10
url: /id/net/aspose.tasks/workingtime/workingtime/
---
## WorkingTime(DateTime, DateTime) {#constructor_1}

Menginisialisasi instance baru dari kelas [`WorkingTime`](../) dengan interval yang memiliki waktu mulai dan selesai yang ditentukan.

```csharp
public WorkingTime(DateTime fromTime, DateTime toTime)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fromTime | DateTime | waktu mulai interval |
| toTime | DateTime | waktu akhir interval |

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

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)

---

## WorkingTime(TimeSpan, TimeSpan) {#constructor_2}

Menginisialisasi instance baru dari kelas [`WorkingTime`](../) dengan item interval yang memiliki waktu mulai dan selesai yang ditentukan.

```csharp
public WorkingTime(TimeSpan fromTime, TimeSpan toTime)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fromTime | TimeSpan | Waktu mulai interval yang direpresentasikan oleh struct TimeSpan. |
| toTime | TimeSpan | Waktu akhir interval yang direpresentasikan oleh struct TimeSpan. |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentException | Ketika toTime kurang dari atau sama dengan argumen toTime atau ketika interval antara fromTime dan toTime lebih dari 24 jam. |

## Contoh

Overload dari konstruktor WorkingTime dapat digunakan untuk menginisialisasi awal dan akhir interval menggunakan TimeSpans:

```csharp
[C#]
var wt = new WorkingTime(new TimeSpan(9, 0, 0), new TimeSpan(18, 0, 0));
```

### Lihat Juga

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)

---

## WorkingTime(int, int) {#constructor}

Menginisialisasi instance baru dari kelas [`WorkingTime`](../) dengan item interval yang memiliki waktu mulai dan selesai yang ditentukan.

```csharp
public WorkingTime(int fromHours, int toHours)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| fromHours | Int32 | Waktu mulai interval direpresentasikan oleh angka bulat jam (0-24). |
| toHours | Int32 | Waktu akhir interval direpresentasikan oleh angka bulat jam (0-24). |

### Pengecualian

| pengecualian | kondisi |
| --- | --- |
| ArgumentException | Ketika toTime kurang dari atau sama dengan argumen toTime atau ketika interval antara fromTime dan toTime lebih dari 24 jam. |

## Contoh

Overload dari konstruktor WorkingTime dapat digunakan untuk menginisialisasi awal dan akhir interval menggunakan jam penuh:

```csharp
[C#]
var wt = new WorkingTime(9, 13);
```

Menampilkan cara memeriksa kesetaraan waktu kerja.

```csharp
var workingTime1 = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 17);

// Kesetaraan kalender diperiksa terhadap tanggal from dan to dari waktu kerja.
Console.WriteLine("Working Time 1 (From): " + workingTime1.From);
Console.WriteLine("Working Time 1 (To): " + workingTime1.To);

Console.WriteLine("Working Time 2 (From): " + workingTime2.From);
Console.WriteLine("Working Time 2 (To): " + workingTime2.To);
Console.WriteLine("Are working times equal: " + workingTime1.Equals(workingTime2));
```

### Lihat Juga

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)


