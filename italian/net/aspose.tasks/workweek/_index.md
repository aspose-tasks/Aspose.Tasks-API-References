---
title: "Classe WorkWeek"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.WorkWeek. Rappresenta la classe WorkWeek"
type: docs
weight: 3640
url: /it/net/aspose.tasks/workweek/
---
## WorkWeek class

Rappresenta la classe WorkWeek

```csharp
public class WorkWeek
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [WorkWeek](workweek/)() | Inizializza una nuova istanza della classe `WorkWeek`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [FromDate](../../aspose.tasks/workweek/fromdate/) { get; set; } | Ottiene o imposta la DateTime di inizio della settimana lavorativa |
| [Name](../../aspose.tasks/workweek/name/) { get; set; } | Ottiene o imposta il Nome della settimana lavorativa |
| [ToDate](../../aspose.tasks/workweek/todate/) { get; set; } | Ottiene o imposta la DateTime di fine della settimana lavorativa |
| [WeekDays](../../aspose.tasks/workweek/weekdays/) { get; } | Ottiene i giorni della settimana. |

## Esempi

Mostra come leggere le informazioni della settimana lavorativa dal progetto.

```csharp
var project = new Project();
var calendar = project.Calendars.Add("Standard");
Calendar.MakeStandardCalendar(calendar);

var item = new WorkWeek();
item.Name = "My Work Week";
item.FromDate = new DateTime(2020, 4, 13, 8, 0, 0);
item.ToDate = new DateTime(2020, 4, 17, 17, 0, 0);
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));
item.WeekDays.Add(new WeekDay(DayType.Saturday));
item.WeekDays.Add(new WeekDay(DayType.Sunday));
calendar.WorkWeeks.Add(item);

Console.WriteLine("Work Week Number: " + calendar.WeekDays.Count);
foreach (var workWeek in calendar.WorkWeeks)
{
    // Visualizza il nome della settimana lavorativa, il nome del calendario padre, le date di inizio e fine
    Console.WriteLine("Name: " + workWeek.Name);
    Console.WriteLine("Parent calendar name: " + calendar.Name);
    Console.WriteLine("From Date: " + workWeek.FromDate);
    Console.WriteLine("To Date: " + workWeek.ToDate);
    Console.WriteLine();

    // Questi dati riguardano il pulsante "Dettagli"; è possibile impostare orari di lavoro speciali per giorni della settimana specifici o persino renderli non lavorativi.
    List<WeekDay> weekDays = workWeek.WeekDays.ToList();
    foreach (var day in weekDays)
    {
        Console.WriteLine(day.DayType.ToString());

        // Puoi inoltre attraversare gli orari di lavoro e visualizzarli.
        foreach (var workingTime in day.WorkingTimes)
        {
            Console.WriteLine(workingTime.From);
            Console.WriteLine(workingTime.To);
        }
    }

    Console.WriteLine();
}
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


