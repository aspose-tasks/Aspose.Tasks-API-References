---
title: "Kelas Calendar"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.Calendar. Mewakili kalender yang digunakan dalam sebuah proyek."
type: docs
weight: 230
url: /id/net/aspose.tasks/calendar/
---
## Calendar class

Mewakili kalender yang digunakan dalam sebuah proyek.

```csharp
public class Calendar : ICalendar
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [BaseCalendar](../../aspose.tasks/calendar/basecalendar/) { get; set; } | Mendapatkan atau mengatur kalender dasar yang menjadi dependensi kalender ini. Hanya berlaku jika kalender bukan kalender dasar. |
| [Exceptions](../../aspose.tasks/calendar/exceptions/) { get; } | Mendapatkan objek CalendarExceptionCollection. Kumpulan pengecualian yang terkait dengan kalender. |
| [Guid](../../aspose.tasks/calendar/guid/) { get; } | Mendapatkan Guid kalender. |
| [IsBaseCalendar](../../aspose.tasks/calendar/isbasecalendar/) { get; } | Mendapatkan nilai yang menunjukkan apakah kalender adalah kalender dasar. |
| [IsBaselineCalendar](../../aspose.tasks/calendar/isbaselinecalendar/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah kalender adalah kalender baseline. |
| [Name](../../aspose.tasks/calendar/name/) { get; set; } | Mendapatkan atau mengatur nama kalender. |
| [PrimaveraProperties](../../aspose.tasks/calendar/primaveraproperties/) { get; } | Mendapatkan objek yang berisi properti khusus Primavera untuk kalender yang dibaca dari format Primavera. |
| [Uid](../../aspose.tasks/calendar/uid/) { get; set; } | Mendapatkan atau mengatur pengidentifikasi unik kalender. |
| [WeekDays](../../aspose.tasks/calendar/weekdays/) { get; } | Mendapatkan WeekDaysCollection untuk kalender ini. Kumpulan hari kerja yang mendefinisikan kalender. |
| [WorkWeeks](../../aspose.tasks/calendar/workweeks/) { get; } | Mendapatkan objek WorkWeekCollections. Kumpulan minggu kerja yang terkait dengan kalender. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| static [Make24HourCalendar](../../aspose.tasks/calendar/make24hourcalendar/)(Calendar) | Membuat Calendar tertentu menjadi Calendar 24Jam. Calendar 24Jam adalah Calendar di mana setiap hari dalam seminggu bekerja dengan jam kerja 24/7. |
| static [MakeNightShiftCalendar](../../aspose.tasks/calendar/makenightshiftcalendar/)(Calendar) | Membuat Kalender yang diberikan menjadi Kalender Shift Malam. |
| static [MakeStandardCalendar](../../aspose.tasks/calendar/makestandardcalendar/)(Calendar) | Membuat kalender standar default. |
| [Delete](../../aspose.tasks/calendar/delete/)() | Menghapus kalender dari proyek. |
| override [Equals](../../aspose.tasks/calendar/equals/)(object) | Kembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork)(DateTime, Duration) | Menghitung tanggal ketika jumlah waktu kerja yang ditentukan akan berlalu menurut kalender. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | Menghitung tanggal ketika jumlah waktu kerja yang ditentukan akan berlalu menurut kalender. |
| override [GetHashCode](../../aspose.tasks/calendar/gethashcode/)() | Mengembalikan kode hash untuk instance kelas. |
| [GetNextWorkingDayStart](../../aspose.tasks/calendar/getnextworkingdaystart/)(DateTime) | Menghitung awal hari kerja berikutnya untuk tanggal yang ditentukan. |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/calendar/getpreviousworkingdayend/)(DateTime) | Menghitung akhir tanggal kerja sebelumnya dari tanggal yang ditentukan. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration)(DateTime, Duration) | Mengembalikan tanggal mulai berdasarkan tanggal selesai dan durasi yang ditentukan. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | Mengembalikan tanggal mulai berdasarkan tanggal selesai dan durasi yang ditentukan. |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/calendar/gettaskfinishdatefromduration/)(Task, TimeSpan) | Menghitung tanggal dan waktu selesai tugas dari tanggal mulainya, bagian-bagian terpisah, dan durasi kerja. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours_1)(DateTime) | Mengembalikan jumlah jam kerja pada tanggal yang ditentukan. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours)(DateTime, DateTime) | Kembalikan WorkUnit - Mulai, Selesai, dan Durasi jam kerja untuk interval tanggal dan waktu yang ditentukan. |
| [GetWorkingHoursTimeSpan](../../aspose.tasks/calendar/getworkinghourstimespan/)(DateTime, DateTime) | Mengembalikan jumlah jam kerja antara tanggal yang ditentukan. |
| [GetWorkingTimes](../../aspose.tasks/calendar/getworkingtimes/)(DateTime) | Mengembalikan [`WorkingTimeCollection`](../workingtimecollection/) dari waktu kerja untuk tanggal yang ditentukan. |
| [GetWorkStart](../../aspose.tasks/calendar/getworkstart/)(DateTime) | Menghitung awal waktu kerja berikutnya mulai dari tanggal dan waktu yang ditentukan. |
| [IsDayWorking](../../aspose.tasks/calendar/isdayworking/)(DateTime) | Menentukan apakah hari yang ditentukan adalah hari kerja menurut kalender. |
| virtual [IsEmpty](../../aspose.tasks/calendar/isempty/)() | Mengembalikan apakah kalender tidak memiliki jam kerja yang didefinisikan. |
| static [GetIntersectionCalendar](../../aspose.tasks/calendar/getintersectioncalendar/)(Calendar, Calendar) | Mendapatkan instance [`ICalendar`](../icalendar/) yang dapat digunakan untuk melakukan perhitungan pada irisan jadwal kerja dari 2 kalender. |

## Catatan

Kalender digunakan untuk mendefinisikan waktu kerja dan non-kerja standar. Proyek harus memiliki satu kalender dasar. Tugas dan sumber daya dapat memiliki kalender non-dasar mereka sendiri yang didasarkan pada kalender dasar.

## Contoh

Cara membuat kalender sederhana dari awal.

```csharp
[C#]
// buat kalender kosong
Calendar calendar = new Calendar("New calendar");
// menambahkan hari kerja default (8 jam kerja dari 9:00 hingga 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
// buat hari kerja baru baru
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
' create empty calendar
Dim calendar As Calendar =  New Calendar("New calendar")
' adds default working days (8 working hours from 9:00 to 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday))
' create new new working day
Dim myWeekDay As WeekDay =  New WeekDay(DayType.Thursday)
' Sets working time. Only time part of DateTime is important
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
' adds weekend
calendar.Days.Add(New WeekDay(DayType.Saturday))
calendar.Days.Add(New WeekDay(DayType.Sunday))
```

Menampilkan cara mendefinisikan kalender baru, menambahkan hari kerja ke dalamnya, dan mendefinisikan waktu kerja untuk hari-hari.

```csharp
var project = new Project();

// Definisikan sebuah kalender
var calendar = project.Calendars.Add("Calendar1");

// Tambahkan hari kerja Senin hingga Kamis dengan jadwal default
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// Setel Jumat sebagai hari kerja pendek
var weekDay = new WeekDay(DayType.Friday);

// Mengatur waktu kerja. Hanya bagian waktu dari DateTime yang penting
var workingTime = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 16);
weekDay.WorkingTimes.Add(workingTime);
weekDay.WorkingTimes.Add(workingTime2);
weekDay.DayWorking = true;
calendar.WeekDays.Add(weekDay);

// bekerja dengan proyek...
```

### Lihat Juga

* interface [ICalendar](../icalendar/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


