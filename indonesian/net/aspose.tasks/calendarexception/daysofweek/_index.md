---
title: "CalendarException.DaysOfWeek"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "CalendarException properti. Mendapatkan DayTypeCollection untuk objek ini. Hari-hari dalam seminggu di mana pengecualian berlaku"
type: docs
weight: 20
url: /id/net/aspose.tasks/calendarexception/daysofweek/
---
## CalendarException.DaysOfWeek property

Mendapatkan DayTypeCollection untuk objek ini. Hari-hari dalam seminggu di mana pengecualian berlaku.

```csharp
public DayTypeCollection DaysOfWeek { get; }
```

## Contoh

Menunjukkan cara mendefinisikan pengecualian kalender berdasarkan hari dalam seminggu.

```csharp
var project = new Project(DataDir + "project_test.mpp");

// Buat kalender
var calendar = project.Calendars.Add("Calendar1");

// Buat pengecualian kalender untuk setiap Jumat
var exception = new CalendarException();
exception.Type = CalendarExceptionType.Weekly;
exception.FromDate = new DateTime(2020, 4, 6);
exception.ToDate = new DateTime(2020, 4, 12);
exception.DaysOfWeek.Add(DayType.Friday);

// periksa bahwa Jumat bersifat pengecualian
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2020, 4, 10)));

// tambahkan pengecualian ke kalender
calendar.Exceptions.Add(exception);
```

### Lihat Juga

* class [DayTypeCollection](../../daytypecollection/)
* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


