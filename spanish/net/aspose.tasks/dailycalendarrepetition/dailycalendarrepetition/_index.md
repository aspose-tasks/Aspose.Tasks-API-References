---
title: "DailyCalendarRepetition.DailyCalendarRepetition"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor DailyCalendarRepetition. Inicializa una nueva instancia de la clase DailyCalendarRepetition"
type: docs
weight: 10
url: /es/net/aspose.tasks/dailycalendarrepetition/dailycalendarrepetition/
---
## DailyCalendarRepetition constructor

Inicializa una nueva instancia de la clase [`DailyCalendarRepetition`](../).

```csharp
public DailyCalendarRepetition()
```

## Ejemplos

Muestra cómo trabajar con repeticiones del patrón de repetición de trabajo diario y un '24 Horas' al crear tareas recurrentes.

```csharp
var project = new Project(DataDir + "Project1.mpp");
var calendar = project.Calendars.Add("24 Hours");
Calendar.Make24HourCalendar(calendar);
var parameters = new RecurringTaskParameters
{
    TaskName = "t1",
    Duration = project.GetDuration(1, TimeUnitType.Day),
    RecurrencePattern = new DailyRecurrencePattern
    {
        Repetition = new DailyCalendarRepetition { RepetitionInterval = 1 },
        RecurrenceRange = new EndByRecurrenceRange
        {
            Start = new DateTime(2018, 7, 2, 0, 0, 0),
            Finish = new DateTime(2018, 7, 8, 16, 0, 0)
        }
    }
};
parameters.SetCalendar(project, "24 Hours");
project.RootTask.Children.Add(parameters);

// trabaja con el proyecto más adelante...
project.Save(OutDir + "CanAddRecurringTask_Days_CalendarDays_24h_Test_out.mpp", SaveFileFormat.Mpp);
```

### Ver también

* class [DailyCalendarRepetition](../)
* namespace [Aspose.Tasks](../../dailycalendarrepetition/)
* assembly [Aspose.Tasks](../../../)


