---
title: "Calendar.Exceptions"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Calendar. Mendapatkan objek CalendarExceptionCollection. Kumpulan pengecualian yang terkait dengan kalender."
type: docs
weight: 50
url: /id/net/aspose.tasks/calendar/exceptions/
---
## Calendar.Exceptions property

Mendapatkan objek CalendarExceptionCollection. Kumpulan pengecualian yang terkait dengan kalender.

```csharp
public CalendarExceptionCollection Exceptions { get; }
```

## Contoh

Menampilkan cara mengambil info tentang pengecualian kalender.

```csharp
var project = new Project(DataDir + "project_RetrieveExceptions_test.mpp");

// Mengulang melalui kalender
foreach (var calendar in project.Calendars)
{
    // Mengakses pengecualian kalender
    foreach (var exception in calendar.Exceptions)
    {
        Console.WriteLine("From: " + exception.FromDate.ToShortDateString());
        Console.WriteLine("To: " + exception.ToDate.ToShortDateString());
    }
}
```

### Lihat Juga

* class [CalendarExceptionCollection](../../calendarexceptioncollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


