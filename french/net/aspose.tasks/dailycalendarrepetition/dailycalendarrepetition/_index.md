---
title: "DailyCalendarRepetition.DailyCalendarRepetition"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Constructeur DailyCalendarRepetition. Initialise une nouvelle instance de la classe DailyCalendarRepetition"
type: docs
weight: 10
url: /fr/net/aspose.tasks/dailycalendarrepetition/dailycalendarrepetition/
---
## DailyCalendarRepetition constructor

Initialise une nouvelle instance de la classe [`DailyCalendarRepetition`](../).

```csharp
public DailyCalendarRepetition()
```

## Exemples

Montre comment travailler avec les répétitions du modèle de répétition de travail quotidien et un '24 Heures' lors de la création de tâches récurrentes.

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

// continuer à travailler avec le projet...
project.Save(OutDir + "CanAddRecurringTask_Days_CalendarDays_24h_Test_out.mpp", SaveFileFormat.Mpp);
```

### Voir aussi

* class [DailyCalendarRepetition](../)
* namespace [Aspose.Tasks](../../dailycalendarrepetition/)
* assembly [Aspose.Tasks](../../../)


