---
title: "Calendar.MakeStandardCalendar"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Calendar. Crea un calendario standard predefinito"
type: docs
weight: 30
url: /it/net/aspose.tasks/calendar/makestandardcalendar/
---
## Calendar.MakeStandardCalendar method

Crea un calendario standard predefinito.

```csharp
public static Calendar MakeStandardCalendar(Calendar calendar)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| calendario | Calendar | Calendario da cui creare il calendario standard. |

### Valore di ritorno

Calendario con 5 giorni lavorativi (lunedì-venerdì) con orari di lavoro 8-12 e 13-17.

## Esempi

Mostra come creare un calendario standard.

```csharp
Project project = new Project();
var calendar = project.Calendars.Add("New calendar");
Calendar.MakeStandardCalendar(calendar);

var workingHours = calendar.GetWorkingTimes(new DateTime(2020, 4, 8));

// mostra ore lavorative
foreach (var wh in workingHours)
{
    Console.WriteLine("From: " + wh.From);
    Console.WriteLine("To: " + wh.To);
}
```

Mostra come creare un calendario con giorni di eccezione.

```csharp
var project = new Project(DataDir + "project_update_test.mpp");
var calendar = project.Calendars.GetByName("Standard");

// Aggiorna le informazioni del calendario
Calendar.MakeStandardCalendar(calendar);
calendar.Name = "Test calendar";
var exception = new CalendarException();
exception.Name = "Exception 1";
exception.FromDate = DateTime.Now;
exception.ToDate = DateTime.Now.AddDays(2);
exception.DayWorking = true;

exception.WorkingTimes.Add(new WorkingTime(9, 13));
exception.WorkingTimes.Add(new WorkingTime(14, 19));
exception.WorkingTimes.Add(new WorkingTime(20, 21));
calendar.Exceptions.Add(exception);

var exception2 = new CalendarException();
exception.Name = "Exception 2";
exception2.FromDate = DateTime.Now.AddDays(7);
exception2.ToDate = exception2.FromDate;
exception2.DayWorking = false;
calendar.Exceptions.Add(exception2);

project.Set(Prj.Calendar, calendar);

project.Save(OutDir + "WriteUpdatedCalendarDataToMPP_out.mpp", SaveFileFormat.Mpp);
```

### Vedi anche

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


