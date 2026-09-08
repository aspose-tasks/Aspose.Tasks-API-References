---
title: "CalendarException.WorkingTimes"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "CalendarException property. Haalt het WorkingTimeCollection-object op of stelt dit in. De verzameling werktijden die de op een weekdag gewerkte tijd definieert. Er moet ten minste één werktijd aanwezig zijn en er mogen niet meer dan vijf zijn."
type: docs
weight: 160
url: /nl/net/aspose.tasks/calendarexception/workingtimes/
---
## CalendarException.WorkingTimes property

Haalt op of stelt het WorkingTimeCollection-object in. De collectie werktijden die de gewerkte tijd op een weekdag definieert. Er moet minstens één werktijd aanwezig zijn, en er kunnen niet meer dan vijf zijn.

```csharp
public WorkingTimeCollection WorkingTimes { get; set; }
```

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

* class [WorkingTimeCollection](../../workingtimecollection/)
* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


