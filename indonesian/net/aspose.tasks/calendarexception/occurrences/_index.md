---
title: "CalendarException.Occurrences"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "CalendarException properti. Mendapatkan atau mengatur jumlah kejadian di mana pengecualian kalender berlaku"
type: docs
weight: 110
url: /id/net/aspose.tasks/calendarexception/occurrences/
---
## CalendarException.Occurrences property

Mendapatkan atau mengatur jumlah kejadian di mana pengecualian kalender berlaku.

```csharp
public int Occurrences { get; set; }
```

## Contoh

Menampilkan cara mendefinisikan pengecualian kalender berdasarkan kejadian.

```csharp
var project = new Project();

// Definisikan sebuah kalender
var calendar = project.Calendars.Add("Calendar1");

// Definisikan pengecualian dan tentukan kejadian
var exception = new CalendarException();
exception.EnteredByOccurrences = true;
exception.Occurrences = 5;
exception.Type = CalendarExceptionType.YearlyByDay;
exception.MonthDay = 22;
exception.Month = Month.April;

// Tambahkan pengecualian ke kalender
calendar.Exceptions.Add(exception);
```

### Lihat Juga

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


