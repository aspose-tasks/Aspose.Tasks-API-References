---
title: "Calendar.WeekDays"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad Calendar. Obtiene WeekDaysCollection para este calendario. La colección de días de la semana que define el calendario"
type: docs
weight: 120
url: /es/net/aspose.tasks/calendar/weekdays/
---
## Calendar.WeekDays property

Obtiene WeekDaysCollection para este calendario. La colección de días laborables que define el calendario.

```csharp
public WeekDayCollection WeekDays { get; }
```

## Ejemplos

Muestra cómo definir un calendar nuevo, agregar días de la semana a él y definir los horarios de trabajo para los días.

```csharp
var project = new Project();

// Definir un calendar
var calendar = project.Calendars.Add("Calendar1");

// Agregar días laborables de lunes a jueves con horarios predeterminados
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// Establecer el viernes como día laborable corto
var weekDay = new WeekDay(DayType.Friday);

// Establece el tiempo de trabajo. Solo la parte de hora de `DateTime` es importante
var workingTime = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 16);
weekDay.WorkingTimes.Add(workingTime);
weekDay.WorkingTimes.Add(workingTime2);
weekDay.DayWorking = true;
calendar.WeekDays.Add(weekDay);

// trabajando con el proyecto...
```

### Ver también

* class [WeekDayCollection](../../weekdaycollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


