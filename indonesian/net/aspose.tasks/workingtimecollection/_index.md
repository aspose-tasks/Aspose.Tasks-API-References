---
title: "Kelas WorkingTimeCollection"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.WorkingTimeCollection. Mewakili kumpulan objek WorkingTimeCollection"
type: docs
weight: 3670
url: /id/net/aspose.tasks/workingtimecollection/
---
## WorkingTimeCollection class

Mewakili kumpulan objek `WorkingTimeCollection`.

```csharp
public class WorkingTimeCollection : IList<WorkingTime>
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Count](../../aspose.tasks/workingtimecollection/count/) { get; } | Mendapatkan jumlah objek yang terkandung dalam objek `WorkingTimeCollection` ini. |
| [Item](../../aspose.tasks/workingtimecollection/item/) { get; set; } | Mengembalikan elemen pada indeks yang ditentukan. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Add](../../aspose.tasks/workingtimecollection/add/)(WorkingTime) | Menambahkan instance WorkingTime baru ke koleksi ini. |
| [Clear](../../aspose.tasks/workingtimecollection/clear/)() | Menghapus semua item [`WorkingTime`](../workingtime/) dari koleksi. |
| [Contains](../../aspose.tasks/workingtimecollection/contains/)(WorkingTime) | Memeriksa apakah elemen yang ditentukan ada dalam List. Melakukan pencarian linier O(n). |
| [CopyTo](../../aspose.tasks/workingtimecollection/copyto/)(WorkingTime[], int) | menyalin isi koleksi ke dalam Array, dimulai pada indeks tertentu |
| [GetEnumerator](../../aspose.tasks/workingtimecollection/getenumerator/)() | Mengembalikan enumerator untuk koleksi ini. |
| [Remove](../../aspose.tasks/workingtimecollection/remove/)(WorkingTime) | Menghapus instance [`WorkingTime`](../workingtime/) dari koleksi ini. |
| [ToList](../../aspose.tasks/workingtimecollection/tolist/)() | Mengonversi objek WorkingTimeCollection menjadi daftar objek [`WorkingTime`](../workingtime/). |

## Contoh

Menampilkan cara bekerja dengan koleksi waktu kerja.

```csharp
var project = new Project();
var calendar = project.Calendars.Add("Custom Calendar");

calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));

var saturdayWorkingTimes = new List<WorkingTime>
{
    new WorkingTime(8, 12),
    new WorkingTime(13, 15)
};
var saturday = new WeekDay(DayType.Saturday);
foreach (var time in saturdayWorkingTimes)
{
    saturday.WorkingTimes.Add(time);
}

// cetak waktu kerja pada hari Sabtu
Console.WriteLine("Saturday working period number: " + saturday.WorkingTimes.Count);
foreach (var time in saturday.WorkingTimes)
{
    Console.WriteLine("From Time: " + time.From);
    Console.WriteLine("To Time: " + time.To);
}

Console.WriteLine();

var sundayWorkingTimes = new List<WorkingTime>
{
    new WorkingTime(10, 15)
};
var sunday = new WeekDay(DayType.Sunday, sundayWorkingTimes);

// cetak waktu kerja pada hari Minggu
List<WorkingTime> workingTimes = sunday.WorkingTimes.ToList();
Console.WriteLine("Sunday working period number: " + workingTimes.Count);
for (var index = 0; index < workingTimes.Count; index++)
{
    var time = workingTimes[index];
    Console.WriteLine("From Time: " + time.From);
    Console.WriteLine("To Time: " + time.To);
}

Console.WriteLine();

calendar.WeekDays.Add(saturday);
calendar.WeekDays.Add(sunday);

foreach (var day in calendar.WeekDays)
{
    Console.WriteLine(day.DayType + ": ");

    // Anda dapat menelusuri lebih lanjut melalui waktu kerja dan menampilkannya.
    foreach (var workingTime in day.WorkingTimes)
    {
        Console.WriteLine(workingTime.From);
        Console.WriteLine(workingTime.To);
    }

    Console.WriteLine();
}
```

### Lihat Juga

* class [WorkingTime](../workingtime/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


