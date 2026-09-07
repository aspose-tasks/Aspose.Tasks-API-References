---
title: "WeekDay.WeekDay"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Konstruktor WeekDay. Menginisialisasi instance baru dari kelas WeekDay dengan tipe hari yang ditentukan"
type: docs
weight: 10
url: /id/net/aspose.tasks/weekday/weekday/
---
## WeekDay(DayType) {#constructor_1}

Menginisialisasi instance baru dari kelas [`WeekDay`](../) dengan tipe hari yang ditentukan.

```csharp
public WeekDay(DayType dayType)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| dayType | DayType | Tipe hari yang ditentukan. |

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

---

## WeekDay(DayType, IEnumerable&lt;WorkingTime&gt;) {#constructor_3}

Menginisialisasi instance baru dari kelas [`WeekDay`](../) dengan tipe hari yang ditentukan dan daftar periode waktu kerja.

```csharp
public WeekDay(DayType dayType, IEnumerable<WorkingTime> workingTimes)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| dayType | DayType | Tipe hari yang ditentukan. |
| workingTimes | IEnumerable`1 | Daftar periode waktu kerja. |

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
* class [WorkingTime](../../workingtime/)
* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)

---

## WeekDay(DayType, params WorkingTime[]) {#constructor_2}

Menginisialisasi instance baru dari kelas [`WeekDay`](../) dengan tipe hari yang ditentukan dan periode waktu kerja.

```csharp
public WeekDay(DayType dayType, params WorkingTime[] workingTimes)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| dayType | DayType | Tipe hari yang ditentukan. |
| workingTimes | WorkingTime[] | Array periode waktu kerja. |

### Lihat Juga

* enum [DayType](../../daytype/)
* class [WorkingTime](../../workingtime/)
* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)

---

## WeekDay() {#constructor}

Menginisialisasi instance baru dari kelas [`WeekDay`](../).

```csharp
public WeekDay()
```

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

* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)


