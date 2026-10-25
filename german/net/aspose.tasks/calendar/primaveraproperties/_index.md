---
title: "Calendar.PrimaveraProperties"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "Calendar-Eigenschaft. Gibt ein Objekt zurück, das Primavera-spezifische Eigenschaften für einen aus Primavera-Formaten gelesenen Kalender enthält"
type: docs
weight: 100
url: /de/net/aspose.tasks/calendar/primaveraproperties/
---
## Calendar.PrimaveraProperties property

Gibt ein Objekt zurück, das Primavera-spezifische Eigenschaften für einen aus Primavera-Formaten gelesenen Kalender enthält.

```csharp
public PrimaveraCalendarProperties PrimaveraProperties { get; }
```

## Beispiele

Zeigt, wie man ein Projekt aus einer Primavera-Datei liest und die Primavera-spezifischen Eigenschaften des Kalenders untersucht.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 4861;

// Gibt ein Projekt mit spezieller UID zurück.
var project = new Project(DataDir + "ScheduleOptions.xer", options);

var calendar = project.Calendars.GetByUid(178);

Console.WriteLine("Hours per day in '{0}' : {1}", calendar.Name, calendar.PrimaveraProperties.HoursPerDay);
```

### Siehe auch

* class [PrimaveraCalendarProperties](../../primaveracalendarproperties/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


