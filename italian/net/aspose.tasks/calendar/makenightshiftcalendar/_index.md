---
title: "Calendar.MakeNightShiftCalendar"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Calendar. Trasforma un Calendar dato in un Night Shift Calendar"
type: docs
weight: 20
url: /it/net/aspose.tasks/calendar/makenightshiftcalendar/
---
## Calendar.MakeNightShiftCalendar method

Crea un Calendario Notturno a partire da un calendario fornito.

```csharp
public static Calendar MakeNightShiftCalendar(Calendar calendar)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| calendario | Calendar | Calendar per creare Night Shift Calendar. |

### Valore di ritorno

Night Shift Calendar.

## Esempi

Mostra come creare un Night Shift Calendar.

```csharp
Project project = new Project();
var calendar = project.Calendars.Add("New calendar");
Calendar.MakeNightShiftCalendar(calendar);

var workingHours = calendar.GetWorkingTimes(new DateTime(2020, 4, 8));

// mostra ore lavorative
foreach (var wh in workingHours)
{
    Console.WriteLine("From: " + wh.From);
    Console.WriteLine("To: " + wh.To);
}
```

Mostra come trasformare un Calendar in un Night Shift Calendar.

```csharp
var project = new Project();

var calendar = project.Calendars.Add("Night Shift");
calendar = Calendar.MakeNightShiftCalendar(calendar);

var workingHours = calendar.GetWorkingTimes(new DateTime(2020, 4, 8));

// mostra ore lavorative
foreach (var wh in workingHours)
{
    Console.WriteLine("From: " + wh.From);
    Console.WriteLine("To: " + wh.To);
}
```

### Vedi anche

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


