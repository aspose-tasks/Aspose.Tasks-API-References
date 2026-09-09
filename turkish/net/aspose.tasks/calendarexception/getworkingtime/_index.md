---
title: "CalendarException.GetWorkingTime"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "CalendarException yöntemi. Bir takvim istisnası için çalışma zamanını döndürür."
type: docs
weight: 200
url: /tr/net/aspose.tasks/calendarexception/getworkingtime/
---
## CalendarException.GetWorkingTime method

Takvim istisnası için çalışma süresini döndürür.

```csharp
public TimeSpan GetWorkingTime()
```

### Dönüş Değeri

Bu takvim istisnası için çalışma zamanını döndürür.

## Örnekler

Bir takvim istisnasının çalışma zamanının nasıl alınacağını gösterir.

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

### Ayrıca Bakınız

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


