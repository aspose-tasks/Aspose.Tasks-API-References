---
title: "Calendar.PrimaveraProperties"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Kalender-eigenschap. Haalt een object op dat Primavera-specifieke eigenschappen bevat voor een kalender gelezen uit Primavera-formaten."
type: docs
weight: 100
url: /nl/net/aspose.tasks/calendar/primaveraproperties/
---
## Calendar.PrimaveraProperties property

Haalt een object op dat Primavera‑specifieke eigenschappen bevat voor een kalender die uit Primavera‑formaten is gelezen.

```csharp
public PrimaveraCalendarProperties PrimaveraProperties { get; }
```

## Voorbeelden

Toont hoe een project uit een Primavera-bestand te lezen en de Primavera-specifieke eigenschappen van de kalender te onderzoeken.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 4861;

// Retourneert project met speciale UID
var project = new Project(DataDir + "ScheduleOptions.xer", options);

var calendar = project.Calendars.GetByUid(178);

Console.WriteLine("Hours per day in '{0}' : {1}", calendar.Name, calendar.PrimaveraProperties.HoursPerDay);
```

### Zie ook

* class [PrimaveraCalendarProperties](../../primaveracalendarproperties/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


