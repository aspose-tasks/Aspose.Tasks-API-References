---
title: "Kelas CalendarExceptionCollection"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Kelas Aspose.Tasks.CalendarExceptionCollection. Mewakili kumpulan objek CalendarException"
type: docs
weight: 260
url: /id/net/aspose.tasks/calendarexceptioncollection/
---
## CalendarExceptionCollection class

Mewakili kumpulan objek [`CalendarException`](../calendarexception/).

```csharp
public class CalendarExceptionCollection : IList<CalendarException>
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Count](../../aspose.tasks/calendarexceptioncollection/count/) { get; } | Mendapatkan jumlah objek yang terdapat dalam objek `CalendarExceptionCollection` ini. |
| [Item](../../aspose.tasks/calendarexceptioncollection/item/) { get; set; } | Mengembalikan elemen pada indeks yang ditentukan. |
| [ParentCalendar](../../aspose.tasks/calendarexceptioncollection/parentcalendar/) { get; } | Mendapatkan kalender induk untuk objek ini. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [Add](../../aspose.tasks/calendarexceptioncollection/add/)(CalendarException) | Menambahkan instance CalendarException ke objek koleksi ini. |
| [AddRange](../../aspose.tasks/calendarexceptioncollection/addrange/)(IEnumerable&lt;CalendarException&gt;) | Menambahkan rentang pengecualian ke daftar internal. |
| [Clear](../../aspose.tasks/calendarexceptioncollection/clear/)() | Menghapus semua item dari `CalendarExceptionCollection`. |
| [GetEnumerator](../../aspose.tasks/calendarexceptioncollection/getenumerator/)() | Mengembalikan enumerator untuk koleksi ini. |
| [Remove](../../aspose.tasks/calendarexceptioncollection/remove/)(CalendarException) | Menghapus instance [`CalendarException`](../calendarexception/) dari koleksi ini. |
| [ToList](../../aspose.tasks/calendarexceptioncollection/tolist/)() | Mengonversi objek CalendarExceptionCollection menjadi daftar objek [`CalendarException`](../calendarexception/). |

## Contoh

Menampilkan cara menggunakan koleksi pengecualian kalender untuk mendefinisikan pengecualian kalender.

```csharp
var project = new Project(DataDir + "project_update_test.mpp");
var calendar = project.Calendars.GetByUid(3);

calendar.Exceptions.Clear();
Calendar.MakeStandardCalendar(calendar);

var exception = new CalendarException();
exception.FromDate = new DateTime(2020, 3, 30, 8, 0, 0);
exception.ToDate = new DateTime(2020, 4, 3, 17, 0, 0);
exception.DayWorking = true;
exception.Name = "Exception 1";

var wt1 = new WorkingTime(9, 13);
var wt2 = new WorkingTime(14, 19);

exception.WorkingTimes.Add(wt1);
exception.WorkingTimes.Add(wt2);
calendar.Exceptions.Add(exception);

var nonWorkingExceptions = new CalendarException[2];
nonWorkingExceptions[0] = new CalendarException();
nonWorkingExceptions[0].FromDate = new DateTime(2020, 4, 13, 8, 0, 0);
nonWorkingExceptions[0].ToDate = new DateTime(2020, 4, 18, 17, 0, 0);
nonWorkingExceptions[0].DayWorking = false;
nonWorkingExceptions[0].Name = "Exception 2";
nonWorkingExceptions[1] = new CalendarException();
nonWorkingExceptions[1].FromDate = new DateTime(2020, 4, 6, 8, 0, 0);
nonWorkingExceptions[1].ToDate = new DateTime(2020, 4, 10, 17, 0, 0);
nonWorkingExceptions[1].DayWorking = false;
nonWorkingExceptions[1].Name = "Exception 3";
calendar.Exceptions.AddRange(nonWorkingExceptions);

Console.WriteLine("Exceptions of calendar {0}: ", calendar.Exceptions.ParentCalendar.Name);
Console.WriteLine("Exceptions count: {0}", calendar.Exceptions.Count);
Console.WriteLine();
foreach (var calendarException in calendar.Exceptions)
{
    Console.WriteLine("Name: " + calendarException.Name);
    Console.WriteLine("From Date: " + calendarException.FromDate);
    Console.WriteLine("To Date: " + calendarException.ToDate);
    Console.WriteLine("Is day working: " + calendarException.DayWorking);
    Console.WriteLine();
}

// hapus semua pengecualian
Console.WriteLine("Remove calendar exceptions...");
List<CalendarException> exceptions = calendar.Exceptions.ToList();
foreach (var calendarException in exceptions)
{
    Console.WriteLine("Remove exception: " + calendarException.Name);
    Console.WriteLine();
    calendar.Exceptions.Remove(calendarException);
}
```

### Lihat Juga

* class [CalendarException](../calendarexception/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


