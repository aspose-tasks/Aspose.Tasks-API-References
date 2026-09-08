---
title: "CalendarCollection.GetByName"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "CalendarCollection methode. Retourneert een agenda met de opgegeven naam."
type: docs
weight: 30
url: /nl/net/aspose.tasks/calendarcollection/getbyname/
---
## CalendarCollection.GetByName method

Retourneert een Calendar met de opgegeven naam.

```csharp
public Calendar GetByName(string name)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| name | String | Naam van een agenda. |

### Retourwaarde

Indien gevonden retourneert het een agenda met een opgegeven naam, anders retourneert het null.

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


