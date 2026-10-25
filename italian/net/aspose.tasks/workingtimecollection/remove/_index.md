---
title: "WorkingTimeCollection.Remove"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "WorkingTimeCollection metodo. Rimuove l'istanza WorkingTime da questa collezione"
type: docs
weight: 80
url: /it/net/aspose.tasks/workingtimecollection/remove/
---
## WorkingTimeCollection.Remove method

Rimuove l'istanza [`WorkingTime`](../../workingtime/) da questa collezione.

```csharp
public bool Remove(WorkingTime item)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| elemento | WorkingTime | L'elemento da rimuovere. |

### Valore di ritorno

true se l'istanza WorkingTime è stata rimossa con successo da questa collezione; altrimenti, false.

## Esempi

Mostra come lavorare con la collezione di orari di lavoro.

```csharp
var project = new Project();
var calendar = project.Calendars.Add("Custom Calendar");

calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));

var saturdayWorkingTimes = new List<WorkingTime>
{
    new WorkingTime(8, 12),
    new WorkingTime(13, 15)
};
var saturday = new WeekDay(DayType.Saturday);
foreach (var time in saturdayWorkingTimes)
{
    saturday.WorkingTimes.Add(time);
}

// stampa gli orari di lavoro del sabato
Console.WriteLine("Saturday working period number: " + saturday.WorkingTimes.Count);
foreach (var time in saturday.WorkingTimes)
{
    Console.WriteLine("From Time: " + time.From);
    Console.WriteLine("To Time: " + time.To);
}

Console.WriteLine();

var sundayWorkingTimes = new List<WorkingTime>
{
    new WorkingTime(10, 15)
};
var sunday = new WeekDay(DayType.Sunday, sundayWorkingTimes);

// stampa gli orari di lavoro della domenica
List<WorkingTime> workingTimes = sunday.WorkingTimes.ToList();
Console.WriteLine("Sunday working period number: " + workingTimes.Count);
for (var index = 0; index < workingTimes.Count; index++)
{
    var time = workingTimes[index];
    Console.WriteLine("From Time: " + time.From);
    Console.WriteLine("To Time: " + time.To);
}

Console.WriteLine();

calendar.WeekDays.Add(saturday);
calendar.WeekDays.Add(sunday);

foreach (var day in calendar.WeekDays)
{
    Console.WriteLine(day.DayType + ": ");

    // Puoi inoltre attraversare gli orari di lavoro e visualizzarli.
    foreach (var workingTime in day.WorkingTimes)
    {
        Console.WriteLine(workingTime.From);
        Console.WriteLine(workingTime.To);
    }

    Console.WriteLine();
}
```

### Vedi anche

* class [WorkingTime](../../workingtime/)
* class [WorkingTimeCollection](../)
* namespace [Aspose.Tasks](../../workingtimecollection/)
* assembly [Aspose.Tasks](../../../)


