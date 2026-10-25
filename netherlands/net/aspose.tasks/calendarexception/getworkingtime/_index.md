---
title: "CalendarException.GetWorkingTime"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "CalendarException method. Retourneert de werktijd voor een agenda-uitzondering."
type: docs
weight: 200
url: /nl/net/aspose.tasks/calendarexception/getworkingtime/
---
## CalendarException.GetWorkingTime method

Retourneert de werktijd voor een kalenderuitzondering.

```csharp
public TimeSpan GetWorkingTime()
```

### Retourwaarde

Retourneert de werktijd voor deze agenda-uitzondering.

## Voorbeelden

Toont hoe je de werktijd van een agenda-uitzondering kunt ophalen.

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

### Zie ook

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


