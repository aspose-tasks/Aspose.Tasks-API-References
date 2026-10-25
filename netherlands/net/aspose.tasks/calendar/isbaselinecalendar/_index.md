---
title: "Calendar.IsBaselineCalendar"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Calendar-eigenschap. Haalt een waarde op of stelt deze in die aangeeft of de calendar een baseline-calendar is"
type: docs
weight: 80
url: /nl/net/aspose.tasks/calendar/isbaselinecalendar/
---
## Calendar.IsBaselineCalendar property

Haalt op of stelt een waarde in die aangeeft of de kalender een baseline‑kalender is.

```csharp
public bool IsBaselineCalendar { get; set; }
```

## Voorbeelden

Toont hoe te controleren of een calendar een baseline calendar is of niet.

```csharp
var project = new Project(DataDir + "IsBaselineCalendar.mpp");

var calendar = project.Calendars.GetByUid(3);

Console.WriteLine("Is baseline calendar: " + calendar.IsBaselineCalendar);
```

### Zie ook

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


