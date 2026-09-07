---
title: "Kelas WeekDayCollection"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.WeekDayCollection. Mewakili koleksi objek WeekDay"
type: docs
weight: 3550
url: /id/net/aspose.tasks/weekdaycollection/
---
## WeekDayCollection class

Mewakili koleksi objek [`WeekDay`](../weekday/).

```csharp
public class WeekDayCollection : IList<WeekDay>
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Count](../../aspose.tasks/weekdaycollection/count/) { get; } | Mendapatkan jumlah objek yang terdapat dalam objek `WeekDayCollection` ini. |
| [Item](../../aspose.tasks/weekdaycollection/item/) { get; set; } | Mendapatkan atau mengatur nilai item pada indeks yang ditentukan. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Add](../../aspose.tasks/weekdaycollection/add/)(WeekDay) | Menambahkan sebuah instance [`WeekDay`](../weekday/) ke objek ini. |
| [Clear](../../aspose.tasks/weekdaycollection/clear/)() | Bersihkan objek WeekDayCollection. |
| [Contains](../../aspose.tasks/weekdaycollection/contains/)(WeekDay) | Memeriksa apakah koleksi berisi [`WeekDay`](../weekday/) yang ditentukan. |
| [CopyTo](../../aspose.tasks/weekdaycollection/copyto/)(WeekDay[], int) | Menyalin konten koleksi ke dalam array pada indeks yang ditentukan. |
| [GetEnumerator](../../aspose.tasks/weekdaycollection/getenumerator/)() | Mengembalikan enumerator untuk koleksi ini. |
| [IndexOf](../../aspose.tasks/weekdaycollection/indexof/)(WeekDay) | Mengembalikan indeks dari [`WeekDay`](../weekday/) yang ditentukan. |
| [Insert](../../aspose.tasks/weekdaycollection/insert/)(int, WeekDay) | Menyisipkan [`WeekDay`](../weekday/) pada indeks yang ditentukan. |
| [Remove](../../aspose.tasks/weekdaycollection/remove/)(WeekDay) | Menghapus [`WeekDay`](../weekday/) yang ditentukan, jika ada. |
| [RemoveAt](../../aspose.tasks/weekdaycollection/removeat/)(int) | Menghapus sebuah item pada indeks yang ditentukan. |
| [ToList](../../aspose.tasks/weekdaycollection/tolist/)() | Mengonversi objek WeekDayCollection menjadi daftar objek [`WeekDay`](../weekday/). |

## Contoh

Menampilkan cara bekerja dengan koleksi hari kerja.

```csharp
var project = new Project();
var calendar = project.Calendars.GetByName("Standard");

// bersihkan hari kerja
calendar.WeekDays.Clear();

calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));
var saturday = WeekDay.CreateDefaultWorkingDay(DayType.Saturday);
var sunday = WeekDay.CreateDefaultWorkingDay(DayType.Sunday);

calendar.WeekDays.Add(saturday);
calendar.WeekDays.Add(sunday);

var fridayWorkingTimes = new List<WorkingTime> { new WorkingTime(new DateTime(2020, 4, 13, 8, 0, 0), new DateTime(2020, 4, 13, 12, 0, 0)) };

var friday = new WeekDay(DayType.Friday, fridayWorkingTimes);
if (calendar.WeekDays.Contains(friday))
{
    calendar.WeekDays.Insert(4, friday);
}

Console.WriteLine("Calendar: " + calendar.Name);
Console.WriteLine("Week days count: " + calendar.WeekDays.Count);
foreach (var day in calendar.WeekDays)
{
    Console.WriteLine(day.DayType);
    foreach (var workingTime in day.WorkingTimes)
    {
        Console.WriteLine("From: " + workingTime.From);
        Console.WriteLine("To: " + workingTime.To);
        Console.WriteLine();
    }
}

// hapus hari Sabtu
calendar.WeekDays.RemoveAt(5);

// hapus hari Minggu
if (calendar.WeekDays.IndexOf(saturday) > 0)
{
    calendar.WeekDays.Remove(sunday);
}

Console.WriteLine("Working times after weekend was removed: ");
List<WeekDay> weekDays = calendar.WeekDays.ToList();
foreach (var day in weekDays)
{
    Console.WriteLine(day.DayType);
    foreach (var workingTime in day.WorkingTimes)
    {
        Console.WriteLine("From: " + workingTime.From);
        Console.WriteLine("To: " + workingTime.To);
        Console.WriteLine();
    }
}

var hour24Calendar = project.Calendars.Add("24 Hours");
Calendar.Make24HourCalendar(hour24Calendar);

// salin hari kerja
var weekDaysArray = new WeekDay[calendar.WeekDays.Count];
calendar.WeekDays.CopyTo(weekDaysArray, 0);

foreach (var weekDay in weekDaysArray)
{
    hour24Calendar.WeekDays.Add(weekDay);
}
```

### Lihat Juga

* class [WeekDay](../weekday/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


