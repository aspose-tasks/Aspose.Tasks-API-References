---
title: "Calendar.Name"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Calendar-eigenschap. Haalt op of stelt de naam van de agenda in"
type: docs
weight: 90
url: /nl/net/aspose.tasks/calendar/name/
---
## Calendar.Name property

Haalt op of stelt de naam van de kalender in.

```csharp
public string Name { get; set; }
```

## Voorbeelden

Toont hoe agenda-informatie op te halen.

```csharp
var project = new Project(DataDir + "RetrieveCalendarInfo.mpp");

// Agenda-informatie ophalen
foreach (var calendar in project.Calendars)
{
    if (calendar.Name == null)
    {
        continue;
    }

    Console.WriteLine("Calendar UID: " + calendar.Uid);
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### Zie ook

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


