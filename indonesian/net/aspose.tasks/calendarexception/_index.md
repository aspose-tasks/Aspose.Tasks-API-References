---
title: "Kelas CalendarException"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.CalendarException. Mewakili periode waktu luar biasa dalam kalender"
type: docs
weight: 250
url: /id/net/aspose.tasks/calendarexception/
---
## CalendarException class

Mewakili periode waktu khusus dalam sebuah kalender.

```csharp
public sealed class CalendarException
```

## Konstruktor

| Nama | Deskripsi |
| --- | --- |
| [CalendarException](calendarexception/)() | Menginisialisasi instance baru dari kelas `CalendarException`. |

## Properti

| Nama | Deskripsi |
| --- | --- |
| [DaysOfWeek](../../aspose.tasks/calendarexception/daysofweek/) { get; } | Mendapatkan DayTypeCollection untuk objek ini. Hari-hari dalam seminggu di mana pengecualian berlaku. |
| [DayWorking](../../aspose.tasks/calendarexception/dayworking/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah tanggal atau tipe hari yang ditentukan merupakan hari kerja. |
| [EnteredByOccurrences](../../aspose.tasks/calendarexception/enteredbyoccurrences/) { get; set; } | Mendapatkan atau mengatur nilai yang menunjukkan apakah rentang pengulangan didefinisikan dengan memasukkan jumlah kejadian. False menunjukkan bahwa rentang pengulangan didefinisikan dengan memasukkan tanggal selesai. |
| [FromDate](../../aspose.tasks/calendarexception/fromdate/) { get; set; } | Mendapatkan atau mengatur awal waktu pengecualian. |
| [Month](../../aspose.tasks/calendarexception/month/) { get; set; } | Mendapatkan atau mengatur bulan di mana pengulangan pengecualian dijadwalkan. |
| [MonthDay](../../aspose.tasks/calendarexception/monthday/) { get; set; } | Mendapatkan atau mengatur hari dalam bulan di mana pengulangan pengecualian dijadwalkan. |
| [MonthItem](../../aspose.tasks/calendarexception/monthitem/) { get; set; } | Mendapatkan atau mengatur item bulan untuk pengulangan pengecualian yang dijadwalkan. |
| [MonthPosition](../../aspose.tasks/calendarexception/monthposition/) { get; set; } | Mendapatkan atau mengatur posisi item bulan dalam satu bulan. |
| [Name](../../aspose.tasks/calendarexception/name/) { get; set; } | Mendapatkan atau mengatur nama pengecualian. |
| [Occurrences](../../aspose.tasks/calendarexception/occurrences/) { get; set; } | Mendapatkan atau mengatur jumlah kejadian di mana pengecualian kalender berlaku. |
| [ParentCalendar](../../aspose.tasks/calendarexception/parentcalendar/) { get; } | Mendapatkan kalender induk untuk objek ini. |
| [Period](../../aspose.tasks/calendarexception/period/) { get; set; } | Mendapatkan atau mengatur periode pengulangan untuk pengecualian. |
| [ToDate](../../aspose.tasks/calendarexception/todate/) { get; set; } | Mendapatkan atau mengatur akhir waktu pengecualian. |
| [Type](../../aspose.tasks/calendarexception/type/) { get; set; } | Mendapatkan atau mengatur tipe pengecualian. |
| [WorkingTimes](../../aspose.tasks/calendarexception/workingtimes/) { get; set; } | Mendapatkan atau mengatur objek WorkingTimeCollection. Kumpulan waktu kerja yang mendefinisikan waktu kerja pada hari kerja. Setidaknya satu waktu kerja harus ada, dan tidak boleh lebih dari lima. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [CheckException](../../aspose.tasks/calendarexception/checkexception/)(DateTime) | Mengembalikan true jika instance struct DateTime yang ditentukan adalah hari pengecualian. |
| [Delete](../../aspose.tasks/calendarexception/delete/)() | Menghapus instance Exception dari objek kalender induk CalendarExceptionCollection. |
| [GetExceptionDates](../../aspose.tasks/calendarexception/getexceptiondates/)() | Mengembalikan tanggal-tanggal di mana pengecualian kalender berlaku. |
| [GetWorkingTime](../../aspose.tasks/calendarexception/getworkingtime/)() | Mengembalikan waktu kerja untuk pengecualian kalender. |

## Contoh

Menampilkan cara menambah/menghapus pengecualian kalender.

```csharp
var project = new Project(DataDir + "project_test.mpp");

// Buat kalender
var calendar = project.Calendars.Add("Calendar1");

// buat pengecualian hari kerja untuk liburan
var exception = new CalendarException();
exception.Name = "New Calendar Exception";
exception.EnteredByOccurrences = false;
exception.FromDate = new DateTime(2009, 12, 24, 0, 0, 0);
exception.ToDate = new DateTime(2009, 12, 31, 23, 59, 0);
exception.Type = CalendarExceptionType.Daily;
exception.Month = Month.December;

exception.DayWorking = false;

// periksa apakah tanggal tersebut bersifat pengecualian
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2009, 12, 26, 8, 0, 0)));

calendar.Exceptions.Add(exception);

// hapus sebuah pengecualian
var cal = project.Calendars.ToList()[0];
if (cal.Exceptions.Count > 1)
{
    var excToRemove = cal.Exceptions[0];
    cal.Exceptions.Remove(excToRemove);
}

// tambahkan sebuah pengecualian
var exception2 = new CalendarException();
exception2.FromDate = new System.DateTime(2009, 1, 1);
exception2.ToDate = new System.DateTime(2009, 1, 3);
cal.Exceptions.Add(exception2);

// cetak pengecualian
foreach (var exc in cal.Exceptions)
{
    Console.WriteLine("Name: " + exc.Name);
    Console.WriteLine("From: " + exc.FromDate.ToShortDateString());
    Console.WriteLine("To: " + exc.ToDate.ToShortDateString());
}
```

### Lihat Juga

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


