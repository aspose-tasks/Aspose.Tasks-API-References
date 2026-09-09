---
title: "CalendarException.WorkingTimes"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "CalendarException özelliği. WorkingTimeCollection nesnesini alır veya ayarlar. Hafta içi çalışılan zamanı tanımlayan çalışma zamanları koleksiyonu. En az bir çalışma zamanı bulunmalı ve beşten fazla olamaz."
type: docs
weight: 160
url: /tr/net/aspose.tasks/calendarexception/workingtimes/
---
## CalendarException.WorkingTimes property

WorkingTimeCollection nesnesini alır veya ayarlar. Haftaiçi çalışılan zamanı tanımlayan çalışma zamanları koleksiyonu. En az bir çalışma zamanı bulunmalı ve beşten fazla olamaz.

```csharp
public WorkingTimeCollection WorkingTimes { get; set; }
```

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

* class [WorkingTimeCollection](../../workingtimecollection/)
* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


