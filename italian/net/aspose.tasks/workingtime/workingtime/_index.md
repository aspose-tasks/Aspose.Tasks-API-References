---
title: "WorkingTime.WorkingTime"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "WorkingTime costruttore. Inizializza una nuova istanza della classe WorkingTime con un intervallo con gli orari di inizio e fine specificati"
type: docs
weight: 10
url: /it/net/aspose.tasks/workingtime/workingtime/
---
## WorkingTime(DateTime, DateTime) {#constructor_1}

Inizializza una nuova istanza della classe [`WorkingTime`](../) con un intervallo con gli orari di inizio e fine specificati.

```csharp
public WorkingTime(DateTime fromTime, DateTime toTime)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fromTime | DateTime | orario di inizio dell'intervallo |
| toTime | DateTime | orario di fine dell'intervallo |

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

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)

---

## WorkingTime(TimeSpan, TimeSpan) {#constructor_2}

Inizializza una nuova istanza della classe [`WorkingTime`](../) con un elemento di intervallo con gli orari di inizio e fine specificati.

```csharp
public WorkingTime(TimeSpan fromTime, TimeSpan toTime)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fromTime | TimeSpan | Orario di inizio dell'intervallo rappresentato dalla struttura TimeSpan. |
| toTime | TimeSpan | Orario di fine dell'intervallo rappresentato dalla struttura TimeSpan. |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentException | Quando toTime è inferiore o uguale all'argomento toTime o quando l'intervallo tra fromTime e toTime è superiore a 24 ore. |

## Esempi

La sovraccarico del costruttore WorkingTime può essere usata per inizializzare l'inizio e la fine dell'intervallo usando TimeSpan:

```csharp
[C#]
var wt = new WorkingTime(new TimeSpan(9, 0, 0), new TimeSpan(18, 0, 0));
```

### Vedi anche

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)

---

## WorkingTime(int, int) {#constructor}

Inizializza una nuova istanza della classe [`WorkingTime`](../) con un elemento di intervallo con gli orari di inizio e fine specificati.

```csharp
public WorkingTime(int fromHours, int toHours)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fromHours | Int32 | L'ora di inizio dell'intervallo è rappresentata da un numero intero di ore (0-24). |
| toHours | Int32 | L'ora di fine dell'intervallo è rappresentata da un numero intero di ore (0-24). |

### Eccezioni

| eccezione | condizione |
| --- | --- |
| ArgumentException | Quando toTime è inferiore o uguale all'argomento toTime o quando l'intervallo tra fromTime e toTime è superiore a 24 ore. |

## Esempi

La sovraccarico del costruttore WorkingTime può essere usata per inizializzare l'inizio e la fine dell'intervallo usando ore intere:

```csharp
[C#]
var wt = new WorkingTime(9, 13);
```

Mostra come verificare l'uguaglianza del tempo di lavoro.

```csharp
var workingTime1 = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 17);

// L'uguaglianza dei calendari è verificata rispetto alle date di inizio e fine del tempo di lavoro.
Console.WriteLine("Working Time 1 (From): " + workingTime1.From);
Console.WriteLine("Working Time 1 (To): " + workingTime1.To);

Console.WriteLine("Working Time 2 (From): " + workingTime2.From);
Console.WriteLine("Working Time 2 (To): " + workingTime2.To);
Console.WriteLine("Are working times equal: " + workingTime1.Equals(workingTime2));
```

### Vedi anche

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)


