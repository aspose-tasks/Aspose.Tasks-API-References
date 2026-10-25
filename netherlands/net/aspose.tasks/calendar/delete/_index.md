---
title: "Calendar.Delete"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Calendar-methode. Verwijdert calendar uit project"
type: docs
weight: 140
url: /nl/net/aspose.tasks/calendar/delete/
---
## Calendar.Delete method

Verwijdert kalender uit project.

```csharp
public void Delete()
```

## Voorbeelden

Toont hoe een calendar uit een project te verwijderen.

```csharp
var project = new Project(DataDir + "BrokenCalendar.mpp");

// haal de calendar op naam
var calendar = project.Calendars.GetByName("Broken Calendar");

// verwijder de agenda
calendar.Delete();
```

### Zie ook

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


