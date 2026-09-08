---
title: "Calendar.MakeStandardCalendar"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Calendar. Crea un calendario estándar predeterminado"
type: docs
weight: 30
url: /es/net/aspose.tasks/calendar/makestandardcalendar/
---
## Calendar.MakeStandardCalendar method

Crea un calendar estándar predeterminado.

```csharp
public static Calendar MakeStandardCalendar(Calendar calendar)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| calendario | Calendar | Calendario del cual crear un calendario estándar. |

### Valor devuelto

Calendario con 5 días laborables (lunes a viernes) con horarios de trabajo 8-12 y 13-17.

## Ejemplos

Muestra cómo crear un calendario estándar.

```csharp
Project project = new Project();
var calendar = project.Calendars.Add("New calendar");
Calendar.MakeStandardCalendar(calendar);

var workingHours = calendar.GetWorkingTimes(new DateTime(2020, 4, 8));

// mostrar horas de trabajo
foreach (var wh in workingHours)
{
    Console.WriteLine("From: " + wh.From);
    Console.WriteLine("To: " + wh.To);
}
```

Muestra cómo crear un calendario con días de excepción.

```csharp
var project = new Project(DataDir + "project_update_test.mpp");
var calendar = project.Calendars.GetByName("Standard");

// Actualizar la información del calendario
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

### Ver también

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


