---
title: "Calendar.PrimaveraProperties"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Calendar. Ottiene un oggetto contenente proprietà specifiche di Primavera per un calendario letto da formati Primavera"
type: docs
weight: 100
url: /it/net/aspose.tasks/calendar/primaveraproperties/
---
## Calendar.PrimaveraProperties property

Ottiene un oggetto contenente proprietà specifiche di Primavera per un calendario letto da formati Primavera.

```csharp
public PrimaveraCalendarProperties PrimaveraProperties { get; }
```

## Esempi

Mostra come leggere un progetto da un file Primavera ed esaminare le proprietà specifiche di Primavera del calendario.

```csharp
var options = new PrimaveraReadOptions();
options.ProjectUid = 4861;

// Restituisce il progetto con UID speciale
var project = new Project(DataDir + "ScheduleOptions.xer", options);

var calendar = project.Calendars.GetByUid(178);

Console.WriteLine("Hours per day in '{0}' : {1}", calendar.Name, calendar.PrimaveraProperties.HoursPerDay);
```

### Vedi anche

* class [PrimaveraCalendarProperties](../../primaveracalendarproperties/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


