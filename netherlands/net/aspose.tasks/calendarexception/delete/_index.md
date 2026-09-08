---
title: "CalendarException.Delete"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "CalendarException method. Verwijdert de Exception-instantie uit het bovenliggende kalenderobject CalendarExceptionCollection"
type: docs
weight: 180
url: /nl/net/aspose.tasks/calendarexception/delete/
---
## CalendarException.Delete method

Verwijdert de Exception-instantie uit het bovenliggende kalenderobject CalendarExceptionCollection.

```csharp
public void Delete()
```

## Voorbeelden

Toont hoe een kalenderuitzondering te verwijderen.

```csharp
var project = new Project(DataDir + "CalendarExceptions.mpp");

var calendar = project.Calendars.ToList()[0];

Console.WriteLine("Calendar Name: " + calendar.Name);
Console.WriteLine("Calendar Exception Count: " + calendar.Exceptions.Count);

// verwijder de uitzondering
calendar.Exceptions[0].Delete();

Console.WriteLine("Calendar Exception Count: " + calendar.Exceptions.Count);
```

### Zie ook

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


