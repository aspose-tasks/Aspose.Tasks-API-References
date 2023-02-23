---
title: Calendar
second_title: Aspose.Tasks untuk Referensi .NET API
description: Merupakan kalender yang digunakan dalam proyek.
type: docs
weight: 230
url: /id/net/aspose.tasks/calendar/
---
## Calendar class

Merupakan kalender yang digunakan dalam proyek.

```csharp
public class Calendar
```

## Properti

| Nama | Keterangan |
| --- | --- |
| [BaseCalendar](../../aspose.tasks/calendar/basecalendar/) { get; set; } | Mendapat atau menyetel kalender dasar tempat kalender ini bergantung. Hanya berlaku jika kalender tersebut bukan kalender dasar. |
| [Exceptions](../../aspose.tasks/calendar/exceptions/) { get; } | Mendapat objek CalendarExceptionCollection. Kumpulan pengecualian yang terkait dengan kalender. |
| [IsBaseCalendar](../../aspose.tasks/calendar/isbasecalendar/) { get; } | Mendapat nilai yang menunjukkan apakah kalender tersebut adalah kalender dasar. |
| [IsBaselineCalendar](../../aspose.tasks/calendar/isbaselinecalendar/) { get; set; } | Mendapat atau menyetel nilai yang menunjukkan apakah kalender adalah kalender garis dasar. |
| [Name](../../aspose.tasks/calendar/name/) { get; set; } | Mendapat atau menyetel nama kalender. |
| [Uid](../../aspose.tasks/calendar/uid/) { get; set; } | Mendapat atau menyetel pengenal unik kalender. |
| [WeekDays](../../aspose.tasks/calendar/weekdays/) { get; } | Mendapat Koleksi Hari Kerja untuk kalender ini. Kumpulan hari kerja yang menentukan kalender. |
| [WorkWeeks](../../aspose.tasks/calendar/workweeks/) { get; } | Mendapat objek WorkWeekCollections. Kumpulan minggu kerja yang terkait dengan kalender. |

## Metode

| Nama | Keterangan |
| --- | --- |
| static [Make24HourCalendar](../../aspose.tasks/calendar/make24hourcalendar/)(Calendar) | Membuat Kalender tertentu menjadi Kalender 24 Jam. Kalender 24 Jam adalah Kalender di mana setiap hari dalam seminggu bekerja dengan jam kerja sepanjang waktu. |
| static [MakeNightShiftCalendar](../../aspose.tasks/calendar/makenightshiftcalendar/)(Calendar) | Menjadikan Kalender tertentu sebagai Kalender Shift Malam. |
| static [MakeStandardCalendar](../../aspose.tasks/calendar/makestandardcalendar/)(Calendar) | Membuat kalender standar default. |
| [Delete](../../aspose.tasks/calendar/delete/)() | Menghapus kalender dari proyek. |
| override [Equals](../../aspose.tasks/calendar/equals/)(object) | Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek tertentu. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork)(DateTime, Duration) | Menghitung tanggal saat jumlah waktu kerja yang ditentukan akan berlalu menurut kalender. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | Menghitung tanggal saat jumlah waktu kerja yang ditentukan akan berlalu menurut kalender. |
| override [GetHashCode](../../aspose.tasks/calendar/gethashcode/)() | Mengembalikan kode hash untuk instance kelas. |
| [GetNextWorkingDayStart](../../aspose.tasks/calendar/getnextworkingdaystart/)(DateTime) | Menghitung hari kerja berikutnya mulai dari tanggal. |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/calendar/getpreviousworkingdayend/)(DateTime) | Menghitung akhir tanggal kerja sebelumnya dari tanggal yang ditentukan. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration)(DateTime, Duration) | Mengembalikan Tanggal Mulai berdasarkan Tanggal Selesai dan Durasi yang ditentukan. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | Mengembalikan Tanggal Mulai berdasarkan Tanggal Selesai dan Durasi yang ditentukan. |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/calendar/gettaskfinishdatefromduration/)(Task, TimeSpan) | Menghitung tanggal dan waktu penyelesaian tugas dari tanggal mulai, membagi bagian, dan durasi. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours_1)(DateTime) | Mengembalikan jumlah jam kerja pada tanggal tersebut. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours)(DateTime, DateTime) | Kembali jam kerja untuk tanggal yang ditentukan. |
| [GetWorkingTimes](../../aspose.tasks/calendar/getworkingtimes/)(DateTime) | Pengembalian[`WorkingTimeCollection`](../workingtimecollection/) waktu kerja untuk tanggal yang ditentukan. |
| [IsDayWorking](../../aspose.tasks/calendar/isdayworking/)(DateTime) | Menentukan apakah hari tersebut adalah hari kerja. |

### Perkataan

Kalender digunakan untuk menentukan waktu kerja dan tidak kerja standar. Proyek harus memiliki satu kalender dasar. Tugas dan sumber daya dapat memiliki kalender non-dasarnya sendiri yang didasarkan pada kalender dasar.

### Contoh

Cara membuat kalender sederhana dari nol.

```csharp
[C#]
// buat kalender kosong
Calendar calendar = new Calendar("New calendar");
// menambahkan hari kerja default (8 jam kerja dari 9:00 hingga 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
// buat hari kerja baru yang baru
WeekDay myWeekDay = new WeekDay(DayType.Thursday);
// Mengatur waktu kerja. Hanya bagian waktu dari DateTime yang penting
    WorkingTime wt1 = new WorkingTime();
    wt1.FromTime = new DateTime(1, 1, 1, 6, 0, 0, 0);
    wt1.ToTime = new DateTime(1, 1, 1, 12, 0, 0, 0);
    WorkingTime wt2 = new WorkingTime();
    wt2.FromTime = new DateTime(1, 1, 1, 14, 0, 0, 0);
    wt2.ToTime = new DateTime(1, 1, 1, 18, 0, 0, 0);
    myWeekDay.WorkingTimes.Add(wt1);
    myWeekDay.WorkingTimes.Add(wt2);
    myWeekDay.DayWorking = true;
calendar.Days.Add(myWeekDay);
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));
// menambahkan akhir pekan
calendar.Days.Add(new WeekDay(DayType.Saturday));
calendar.Days.Add(new WeekDay(DayType.Sunday));
```

```csharp
[VB]
' buat kalender kosong
Dim calendar As Calendar =  New Calendar("New calendar")
' menambahkan hari kerja default (8 jam kerja dari 9:00 hingga 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday))
' buat hari kerja baru yang baru
Dim myWeekDay As WeekDay =  New WeekDay(DayType.Thursday)
' Mengatur waktu kerja. Hanya bagian waktu dari DateTime yang penting
    Dim wt1 As WorkingTime =  New WorkingTime()
    wt1.FromTime = New DateTime(1, 1, 1, 6, 0, 0, 0)
    wt1.ToTime = New DateTime(1, 1, 1, 12, 0, 0, 0)
    Dim wt2 As WorkingTime =  New WorkingTime()
    wt2.FromTime = New DateTime(1, 1, 1, 14, 0, 0, 0)
    wt2.ToTime = New DateTime(1, 1, 1, 18, 0, 0, 0)
    myWeekDay.WorkingTimes.Add(wt1)
    myWeekDay.WorkingTimes.Add(wt2)
    myWeekDay.DayWorking = True
calendar.Days.Add(myWeekDay)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday))
' menambahkan akhir pekan
calendar.Days.Add(New WeekDay(DayType.Saturday))
calendar.Days.Add(New WeekDay(DayType.Sunday))
```

### Lihat juga

* ruang nama [Aspose.Tasks](../../aspose.tasks/)
* perakitan [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
