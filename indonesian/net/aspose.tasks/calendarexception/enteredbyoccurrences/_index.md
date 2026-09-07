---
title: "CalendarException.EnteredByOccurrences"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti CalendarException. Mendapatkan atau mengatur nilai yang menunjukkan apakah rentang pengulangan didefinisikan dengan memasukkan jumlah kejadian. False menunjukkan bahwa rentang pengulangan didefinisikan dengan memasukkan tanggal selesai."
type: docs
weight: 40
url: /id/net/aspose.tasks/calendarexception/enteredbyoccurrences/
---
## CalendarException.EnteredByOccurrences property

Mendapatkan atau mengatur nilai yang menunjukkan apakah rentang pengulangan didefinisikan dengan memasukkan jumlah kejadian. False menunjukkan bahwa rentang pengulangan didefinisikan dengan memasukkan tanggal selesai.

```csharp
public bool EnteredByOccurrences { get; set; }
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


