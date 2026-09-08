---
title: "CalendarCollection.GetByUid"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "CalendarCollection-methode. Retourneert een agenda met de opgegeven UID"
type: docs
weight: 40
url: /nl/net/aspose.tasks/calendarcollection/getbyuid/
---
## CalendarCollection.GetByUid method

Retourneert een Calendar met de opgegeven UID.

```csharp
public Calendar GetByUid(int uid)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| uid | Int32 | UID van een agenda. |

### Retourwaarde

Agenda met een opgegeven UID.

## Voorbeelden

Toont hoe agenda's op te halen op naam of op ID.

```csharp
var project = new Project(DataDir + "Project5.mpp");

var calendarByName = project.Calendars.GetByName("TestCalendar");
var calendarByUid = project.Calendars.GetByUid(4);

Console.WriteLine("Calendar Name: " + calendarByName.Name);
Console.WriteLine("Calendar Name: " + calendarByUid.Name);
Console.WriteLine("Are calendars equals: " + calendarByName.Equals(calendarByUid));
```

### Zie ook

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


