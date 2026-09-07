---
title: "Classe WorkingTime"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.WorkingTime. Rappresenta un orario di lavoro durante un giorno della settimana."
type: docs
weight: 3660
url: /it/net/aspose.tasks/workingtime/
---
## WorkingTime class

Rappresenta un orario di lavoro durante un giorno della settimana.

```csharp
public class WorkingTime
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [WorkingTime](workingtime/#constructor_1)(DateTime, DateTime) | Inizializza una nuova istanza della classe `WorkingTime` con un intervallo con gli orari di inizio e fine specificati. |
| [WorkingTime](workingtime/#constructor)(int, int) | Inizializza una nuova istanza della classe `WorkingTime` con un elemento di intervallo con gli orari di inizio e fine specificati. |
| [WorkingTime](workingtime/#constructor_2)(TimeSpan, TimeSpan) | Inizializza una nuova istanza della classe `WorkingTime` con un elemento di intervallo con gli orari di inizio e fine specificati. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [From](../../aspose.tasks/workingtime/from/) { get; } | Ottiene l'inizio di un orario di lavoro. |
| [To](../../aspose.tasks/workingtime/to/) { get; } | Ottiene la fine di un orario di lavoro. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [Equals](../../aspose.tasks/workingtime/equals/)(object) | Verifica che gli oggetti siano uguali. |
| override [GetHashCode](../../aspose.tasks/workingtime/gethashcode/)() | Restituisce un valore di hash code per l'istanza della classe `WorkingTime`. |

## Esempi

Mostra come lavorare con le informazioni sull'orario di lavoro.

```csharp
public void WorkWithWorkingTime()
{
    var project = new Project();
    var calendar = CreateCalendar(project);
    project.Set(Prj.Calendar, calendar);

    Console.WriteLine("Work Week Number: " + calendar.WeekDays.Count);

    // Questi dati riguardano il pulsante "Dettagli"; è possibile impostare orari di lavoro speciali per giorni della settimana specifici o persino renderli non lavorativi.
    List<WeekDay> weekDays = calendar.WeekDays.ToList();
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
}

public static Calendar CreateCalendar(Project project)
{
    var calendar = project.Calendars.Add("MyCalendar", project.Calendars.GetByName("Standard"));
    var workingTimes = new List<WorkingTime>
                           {
                               new WorkingTime(new DateTime(1, 1, 1, 9, 0, 0), new DateTime(1, 1, 1, 12, 0, 0)),
                               new WorkingTime(new DateTime(1, 1, 1, 13, 0, 0), new DateTime(1, 1, 1, 18, 0, 0))
                           };

    calendar.WeekDays.Add(new WeekDay(DayType.Monday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Tuesday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Wednesday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Thursday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Friday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
    calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

    return calendar;
}
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


