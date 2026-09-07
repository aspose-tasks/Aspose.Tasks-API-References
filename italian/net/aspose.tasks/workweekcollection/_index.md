---
title: "Classe WorkWeekCollection"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.WorkWeekCollection. Rappresenta una raccolta di oggetti WorkWeek"
type: docs
weight: 3650
url: /it/net/aspose.tasks/workweekcollection/
---
## WorkWeekCollection class

Rappresenta una raccolta di oggetti [`WorkWeek`](../workweek/).

```csharp
public class WorkWeekCollection : IList<WorkWeek>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.tasks/workweekcollection/count/) { get; } | Restituisce il numero di oggetti contenuti in questo oggetto `WorkWeekCollection`. |
| [Item](../../aspose.tasks/workweekcollection/item/) { get; set; } | Restituisce l'elemento all'indice specificato. |
| [ParentCalendar](../../aspose.tasks/workweekcollection/parentcalendar/) { get; } | Restituisce il calendario padre. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.tasks/workweekcollection/add/)(WorkWeek) | Aggiunge un'istanza di WorkWeek a questo oggetto di raccolta. |
| [GetEnumerator](../../aspose.tasks/workweekcollection/getenumerator/)() | Restituisce un enumeratore per questa collezione. |
| [ToList](../../aspose.tasks/workweekcollection/tolist/)() | Converte l'oggetto WorkWeekCollection in un elenco di oggetti [`WorkWeek`](../workweek/). |

## Esempi

Mostra come creare una settimana lavorativa personalizzata per un calendario.

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

Console.WriteLine("Work Weeks Count: " + calendar.WorkWeeks.Count);
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

* class [WorkWeek](../workweek/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


