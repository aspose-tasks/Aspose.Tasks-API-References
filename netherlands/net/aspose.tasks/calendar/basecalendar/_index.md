---
title: "Calendar.BaseCalendar"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Calendar-eigenschap. Haalt op of stelt de basisagenda in waarop deze agenda afhankelijk is. Alleen van toepassing als de agenda geen basisagenda is."
type: docs
weight: 40
url: /nl/net/aspose.tasks/calendar/basecalendar/
---
## Calendar.BaseCalendar property

Haalt op of stelt de basis‑kalender in waarop deze kalender afhankelijk is. Alleen van toepassing als de kalender geen basis‑kalender is.

```csharp
public Calendar BaseCalendar { get; set; }
```

## Voorbeelden

Toont hoe te werken met een basisagenda van de agenda van de resource.

```csharp
var project = new Project(DataDir + "ResourceCalendar.mpp");
var resource = project.Resources.Add("Resource1");

// Voeg een standaardagenda toe en wijs toe aan een resource
var calendar = project.Calendars.Add("Resource1");
resource.Set(Rsc.Calendar, calendar);

// Toon basiskalendernaam voor alle resources
foreach (var rsc in project.Resources)
{
    if (rsc.Get(Rsc.Name) != null)
    {
        Console.WriteLine(rsc.Get(Rsc.Calendar).BaseCalendar.Name);
    }
}
```

### Zie ook

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


