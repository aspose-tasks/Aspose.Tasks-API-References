---
title: "CalendarException.Delete"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "CalendarException metode. Menghapus instance Exception dari objek kalender induk CalendarExceptionCollection"
type: docs
weight: 180
url: /id/net/aspose.tasks/calendarexception/delete/
---
## CalendarException.Delete method

Menghapus instance Exception dari objek kalender induk CalendarExceptionCollection.

```csharp
public void Delete()
```

## Contoh

Menunjukkan cara menghapus pengecualian kalender.

```csharp
var project = new Project(DataDir + "CalendarExceptions.mpp");

var calendar = project.Calendars.ToList()[0];

Console.WriteLine("Calendar Name: " + calendar.Name);
Console.WriteLine("Calendar Exception Count: " + calendar.Exceptions.Count);

// hapus pengecualian
calendar.Exceptions[0].Delete();

Console.WriteLine("Calendar Exception Count: " + calendar.Exceptions.Count);
```

### Lihat Juga

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


