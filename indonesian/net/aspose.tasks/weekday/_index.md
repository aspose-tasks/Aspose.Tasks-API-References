---
title: "Kelas WeekDay"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.WeekDay. Mewakili hari kerja yang dapat mendefinisikan hari reguler dalam seminggu atau hari pengecualian dalam kalender."
type: docs
weight: 3540
url: /id/net/aspose.tasks/weekday/
---
## WeekDay class

Mewakili hari kerja yang dapat mendefinisikan hari reguler dalam seminggu atau hari pengecualian dalam kalender.

```csharp
public class WeekDay
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [WeekDay](weekday/#constructor)() | Menginisialisasi instance baru dari kelas `WeekDay`. |
| [WeekDay](weekday/#constructor_1)(DayType) | Menginisialisasi instance baru dari kelas `WeekDay` dengan tipe hari yang ditentukan. |
| [WeekDay](weekday/#constructor_3)(DayType, IEnumerable&lt;WorkingTime&gt;) | Menginisialisasi instance baru dari kelas `WeekDay` dengan tipe hari yang ditentukan dan daftar periode waktu kerja. |
| [WeekDay](weekday/#constructor_2)(DayType, params WorkingTime[]) | Menginisialisasi instance baru dari kelas `WeekDay` dengan tipe hari yang ditentukan dan periode waktu kerja. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [DayType](../../aspose.tasks/weekday/daytype/) { get; } | Mendapatkan tipe hari. |
| [DayWorking](../../aspose.tasks/weekday/dayworking/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah tanggal atau tipe hari yang ditentukan merupakan hari kerja. |
| [FromDate](../../aspose.tasks/weekday/fromdate/) { get; set; } | Mendapatkan atau mengatur awal waktu pengecualian. |
| [ToDate](../../aspose.tasks/weekday/todate/) { get; set; } | Mendapatkan atau mengatur akhir waktu pengecualian. |
| [WorkingTimes](../../aspose.tasks/weekday/workingtimes/) { get; } | Mendapatkan WorkingTimeCollection untuk instance WeekDay ini. Koleksi waktu kerja yang mendefinisikan waktu kerja pada hari kerja tersebut. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| static [CreateDefaultWorkingDay](../../aspose.tasks/weekday/createdefaultworkingday/)(DayType) | Membuat hari kerja default. |
| [Clone](../../aspose.tasks/weekday/clone/)() | Mengembalikan salinan mendalam dari hari kerja. |
| override [Equals](../../aspose.tasks/weekday/equals/)(object) | Kembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| override [GetHashCode](../../aspose.tasks/weekday/gethashcode/)() | Mengembalikan nilai kode hash untuk instance kelas `WeekDay`. |
| [GetWorkingTime](../../aspose.tasks/weekday/getworkingtime/)() | Mengembalikan waktu kerja untuk hari kerja. |
| static [CastToDayType](../../aspose.tasks/weekday/casttodaytype/)(DayOfWeek) | Mengubah DayOfWeek .Net menjadi [`DayType`](./daytype/). |
| static [SetDefaultWorkingTime](../../aspose.tasks/weekday/setdefaultworkingtime/)(WeekDay) | Mengatur periode waktu default untuk hari kerja yang ditentukan. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


