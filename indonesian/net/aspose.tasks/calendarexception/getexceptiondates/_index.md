---
title: "CalendarException.GetExceptionDates"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode CalendarException. Mengembalikan tanggal-tanggal di mana pengecualian kalender berlaku"
type: docs
weight: 190
url: /id/net/aspose.tasks/calendarexception/getexceptiondates/
---
## CalendarException.GetExceptionDates method

Mengembalikan tanggal-tanggal di mana pengecualian kalender berlaku.

```csharp
public IEnumerable<DateTime> GetExceptionDates()
```

### Nilai Kembali

Mengembalikan koleksi tanggal pengecualian yang berlaku untuk pengecualian kalender.

## Contoh

Menunjukkan cara mendapatkan tanggal di mana pengecualian kalender tertentu efektif.

```csharp
Project project = new Project(DataDir + "CalendarExceptions.mpp");
Calendar calendar = project.Calendars.GetByUid(1);
CalendarException calendarException = calendar.Exceptions[0];

foreach (var date in calendarException.GetExceptionDates())
{
    Console.WriteLine(date);
}
```

### Lihat Juga

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


