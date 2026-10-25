---
title: "Calendar.IsBaselineCalendar"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Calendar. Ottiene o imposta un valore che indica se il calendario è un calendario di baseline"
type: docs
weight: 80
url: /it/net/aspose.tasks/calendar/isbaselinecalendar/
---
## Calendar.IsBaselineCalendar property

Ottiene o imposta un valore che indica se il calendario è un calendario di baseline.

```csharp
public bool IsBaselineCalendar { get; set; }
```

## Esempi

Mostra come verificare se un calendario è un calendario di baseline o meno.

```csharp
var project = new Project(DataDir + "IsBaselineCalendar.mpp");

var calendar = project.Calendars.GetByUid(3);

Console.WriteLine("Is baseline calendar: " + calendar.IsBaselineCalendar);
```

### Vedi anche

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


