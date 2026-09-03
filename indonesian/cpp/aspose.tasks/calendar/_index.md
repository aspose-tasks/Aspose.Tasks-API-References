---
title: "kelas Aspose::Tasks::Calendar"
linktitle: "Kalender"
articleTitle: "Kalender"
second_title: "Aspose.Tasks untuk C++"
description: "Mewakili kalender yang digunakan dalam sebuah proyek."
type: docs
weight: 10
url: /id/cpp/aspose.tasks/calendar/
---

## Calendar class

**Inherits:** Aspose::Tasks::ICalendar

Mewakili kalender yang digunakan dalam sebuah proyek.

Cara membuat kalender sederhana dari awal.

```cpp
[C#]
// buat kalender kosong
Calendar calendar = new Calendar("New calendar");
// menambahkan hari kerja default (8 jam kerja dari 9:00 hingga 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
// buat hari kerja baru
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

```cpp
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

Kalender digunakan untuk mendefinisikan waktu kerja standar dan non-kerja. Proyek harus memiliki satu kalender dasar. Tugas dan sumber daya dapat memiliki kalender non-dasar mereka sendiri yang berbasis pada kalender dasar.

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Delete](./delete/) | Menghapus kalender dari proyek. |
| [Equals](./equals/) | Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan. |
| [get_BaseCalendar](./get_basecalendar/) | Mendapatkan kalender dasar tempat kalender ini bergantung. Hanya berlaku jika kalender bukan kalender dasar. |
| [get_Exceptions](./get_exceptions/) | Mendapatkan objek CalendarExceptionCollection. Kumpulan pengecualian yang terkait dengan kalender. |
| [get_Guid](./get_guid/) | Mendapatkan Guid kalender. |
| [get_IsBaseCalendar](./get_isbasecalendar/) | Mendapatkan nilai yang menunjukkan apakah kalender adalah kalender dasar. |
| [get_IsBaselineCalendar](./get_isbaselinecalendar/) | Mendapatkan nilai yang menunjukkan apakah kalender adalah kalender baseline. |
| [get_Name](./get_name/) | Mendapatkan nama kalender. |
| [get_Uid](./get_uid/) | Mendapatkan pengidentifikasi unik kalender. |
| [get_WeekDays](./get_weekdays/) | Mendapatkan WeekDaysCollection untuk kalender ini. Kumpulan hari kerja yang mendefinisikan kalender. |
| [get_WorkWeeks](./get_workweeks/) | Mendapatkan objek WorkWeekCollections. Kumpulan minggu kerja yang terkait dengan kalender. |
| [GetFinishDateByStartAndWork (2 overloads)](./getfinishdatebystartandwork/) | Menghitung tanggal ketika jumlah waktu kerja yang ditentukan akan berlalu menurut kalender. |
| [GetHashCode](./gethashcode/) | Mengembalikan kode hash untuk instance kelas. |
| [GetIntersectionCalendar](./getintersectioncalendar/) | Mendapatkan instance ICalendar yang dapat digunakan untuk melakukan perhitungan pada irisan jadwal kerja dari 2 kalender. |
| [GetNextWorkingDayStart](./getnextworkingdaystart/) | Menghitung awal hari kerja berikutnya untuk tanggal yang ditentukan. |
| [GetPreviousWorkingDayEnd](./getpreviousworkingdayend/) | Menghitung akhir tanggal kerja sebelumnya dari tanggal yang ditentukan. |
| [GetStartDateFromFinishAndDuration (2 overloads)](./getstartdatefromfinishandduration/) | Mengembalikan tanggal mulai berdasarkan tanggal selesai dan durasi yang ditentukan. |
| [GetTaskFinishDateFromDuration](./gettaskfinishdatefromduration/) | Menghitung tanggal dan waktu selesai tugas dari tanggal mulai, bagian-bagian terpisah, dan durasi kerja. |
| [GetWorkingHours (2 overloads)](./getworkinghours/) | Mengembalikan jumlah jam kerja pada tanggal yang ditentukan. |
| [GetWorkingHoursTimeSpan](./getworkinghourstimespan/) | Mengembalikan jumlah jam kerja antara tanggal yang ditentukan. |
| [GetWorkingTimes](./getworkingtimes/) | Mengembalikan WorkingTimeCollection dari waktu kerja untuk tanggal yang ditentukan. |
| [GetWorkStart](./getworkstart/) | Menghitung awal waktu kerja berikutnya mulai dari tanggal dan waktu yang ditentukan. |
| [IsDayWorking](./isdayworking/) | Menentukan apakah hari yang ditentukan adalah hari kerja menurut kalender. |
| [IsEmpty](./isempty/) | Mengembalikan apakah kalender tidak memiliki jam kerja yang didefinisikan. |
| [Make24HourCalendar](./make24hourcalendar/) | Membuat Calendar tertentu menjadi 24Hour Calendar. 24Hours Calendar adalah Calendar di mana setiap hari dalam seminggu bekerja dengan jam kerja 24 jam. |
| [MakeNightShiftCalendar](./makenightshiftcalendar/) | Membuat Calendar tertentu menjadi Night Shift Calendar. |
| [MakeStandardCalendar](./makestandardcalendar/) | Membuat kalender standar default. |
| [set_BaseCalendar](./set_basecalendar/) | Menetapkan kalender dasar tempat kalender ini bergantung. Hanya berlaku jika kalender bukan kalender dasar. |
| [set_IsBaselineCalendar](./set_isbaselinecalendar/) | Menetapkan nilai yang menunjukkan apakah kalender adalah kalender baseline. |
| [set_Name](./set_name/) | Menetapkan nama kalender. |
| [set_Uid](./set_uid/) | Menetapkan pengidentifikasi unik kalender. |

