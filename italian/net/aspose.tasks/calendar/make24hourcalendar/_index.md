---
title: "Calendar.Make24HourCalendar"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Calendar. Trasforma un calendario dato in un Calendario 24Ore. Il Calendario 24Ore è un calendario in cui ogni giorno della settimana è lavorativo con ore di lavoro 24 ore su 24."
type: docs
weight: 10
url: /it/net/aspose.tasks/calendar/make24hourcalendar/
---
## Calendar.Make24HourCalendar method

Trasforma un calendario dato in un Calendario 24Ore. Il Calendario 24Ore è un calendario in cui ogni giorno della settimana è lavorativo con orari di lavoro 24 ore su 24.

```csharp
public static Calendar Make24HourCalendar(Calendar calendar)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| calendario | Calendar | Calendario per creare un Calendario di 24 ore da. |

### Valore di ritorno

Calendario 24 ore.

## Esempi

Mostra come creare un calendario di 24 ore.

```csharp
Project project = new Project();
var calendar = project.Calendars.Add("New calendar");
Calendar.Make24HourCalendar(calendar);

var workingHours = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0));

// Verranno stampate 24 ore
Console.WriteLine("Hours: " + workingHours.TotalHours);
```

Mostra come trasformare un nuovo calendario in un calendario di 24 ore.

```csharp
var project = new Project();

var calendar = project.Calendars.Add("24 Hours");
calendar = Calendar.Make24HourCalendar(calendar);

var workingHours = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0));

// Verranno stampate 24 ore
Console.WriteLine("Hours: " + workingHours.TotalHours);
```

### Vedi anche

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


