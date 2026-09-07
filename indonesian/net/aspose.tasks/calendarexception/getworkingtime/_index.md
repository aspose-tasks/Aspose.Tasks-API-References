---
title: "CalendarException.GetWorkingTime"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode CalendarException. Mengembalikan waktu kerja untuk pengecualian kalender."
type: docs
weight: 200
url: /id/net/aspose.tasks/calendarexception/getworkingtime/
---
## CalendarException.GetWorkingTime method

Mengembalikan waktu kerja untuk pengecualian kalender.

```csharp
public TimeSpan GetWorkingTime()
```

### Nilai Kembali

Mengembalikan waktu kerja untuk pengecualian kalender ini.

## Contoh

Menampilkan cara mendapatkan waktu kerja dari pengecualian kalender.

```csharp
var project = new Project(DataDir + "CalendarExceptions.mpp");

var calendar = project.Calendars.ToList()[0];
var exception = calendar.Exceptions[0];

Console.WriteLine("Calendar Name: " + calendar.Name);
Console.WriteLine("Calendar Exception Count: " + calendar.Exceptions.Count);
Console.WriteLine("Calendar Exception Name: " + exception.Name);
Console.WriteLine();

var workingTime = exception.GetWorkingTime();
Console.WriteLine("Exception Working Time: " + workingTime);

foreach (var time in exception.WorkingTimes)
{
    Console.WriteLine("Working Time Start: " + time.From);
    Console.WriteLine("Working Time Finish: " + time.To);
}
```

### Lihat Juga

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


