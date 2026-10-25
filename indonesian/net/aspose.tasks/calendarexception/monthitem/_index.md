---
title: "CalendarException.MonthItem"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "CalendarException properti. Mendapatkan atau mengatur item bulan untuk mana rekursi pengecualian dijadwalkan"
type: docs
weight: 80
url: /id/net/aspose.tasks/calendarexception/monthitem/
---
## CalendarException.MonthItem property

Mendapatkan atau mengatur item bulan untuk pengulangan pengecualian yang dijadwalkan.

```csharp
public MonthItemType MonthItem { get; set; }
```

## Contoh

Menampilkan cara mendefinisikan pengecualian kalender berdasarkan hari bulan.

```csharp
var project = new Project(DataDir + "project_test.mpp");

// Buat kalender
var calendar = project.Calendars.Add("Calendar1");

// Buat pengecualian kalender untuk setiap Jumat
var exception = new CalendarException();
exception.Type = CalendarExceptionType.MonthlyByDay;
exception.FromDate = new DateTime(2010, 1, 1);
exception.ToDate = new DateTime(2020, 12, 31);
exception.Month = Month.December;
exception.MonthDay = 1;
exception.MonthItem = MonthItemType.Undefined;
exception.MonthPosition = MonthPosition.Last;
exception.Period = 5;

// Periksa bahwa Jumat aa adalah pengecualian
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2012, 12, 1)));

// tambahkan pengecualian ke kalender
calendar.Exceptions.Add(exception);
```

### Lihat Juga

* enum [MonthItemType](../../monthitemtype/)
* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


