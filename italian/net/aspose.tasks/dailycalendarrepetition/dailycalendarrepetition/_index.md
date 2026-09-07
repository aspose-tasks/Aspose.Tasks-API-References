---
title: "DailyCalendarRepetition.DailyCalendarRepetition"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "DailyCalendarRepetition costruttore. Inizializza una nuova istanza della classe DailyCalendarRepetition"
type: docs
weight: 10
url: /it/net/aspose.tasks/dailycalendarrepetition/dailycalendarrepetition/
---
## DailyCalendarRepetition constructor

Inizializza una nuova istanza della classe [`DailyCalendarRepetition`](../).

```csharp
public DailyCalendarRepetition()
```

## Esempi

Mostra come lavorare con le ripetizioni del modello di ripetizione del lavoro giornaliero e un '24 Ore' durante la creazione di attività ricorrenti.

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

// continua a lavorare sul progetto...
project.Save(OutDir + "CanAddRecurringTask_Days_CalendarDays_24h_Test_out.mpp", SaveFileFormat.Mpp);
```

### Vedi anche

* class [DailyCalendarRepetition](../)
* namespace [Aspose.Tasks](../../dailycalendarrepetition/)
* assembly [Aspose.Tasks](../../../)


