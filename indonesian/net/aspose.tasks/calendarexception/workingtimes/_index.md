---
title: "CalendarException.WorkingTimes"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti CalendarException. Mendapatkan atau mengatur objek WorkingTimeCollection. Kumpulan waktu kerja yang menentukan waktu kerja pada hari kerja. Setidaknya satu waktu kerja harus ada dan tidak boleh lebih dari lima."
type: docs
weight: 160
url: /id/net/aspose.tasks/calendarexception/workingtimes/
---
## CalendarException.WorkingTimes property

Mendapatkan atau mengatur objek WorkingTimeCollection. Kumpulan waktu kerja yang mendefinisikan waktu kerja pada hari kerja. Setidaknya satu waktu kerja harus ada, dan tidak boleh lebih dari lima.

```csharp
public WorkingTimeCollection WorkingTimes { get; set; }
```

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

* class [WorkingTimeCollection](../../workingtimecollection/)
* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


