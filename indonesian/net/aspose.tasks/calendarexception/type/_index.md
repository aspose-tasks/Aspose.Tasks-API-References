---
title: "CalendarException.Type"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti CalendarException. Mendapatkan atau mengatur tipe pengecualian."
type: docs
weight: 150
url: /id/net/aspose.tasks/calendarexception/type/
---
## CalendarException.Type property

Mendapatkan atau mengatur tipe pengecualian.

```csharp
public CalendarExceptionType Type { get; set; }
```

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

* enum [CalendarExceptionType](../../calendarexceptiontype/)
* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


