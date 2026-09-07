---
title: "Classe WorkingTimeCollection"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.WorkingTimeCollection. Rappresenta una collezione di oggetti WorkingTimeCollection"
type: docs
weight: 3670
url: /it/net/aspose.tasks/workingtimecollection/
---
## WorkingTimeCollection class

Rappresenta una collezione di oggetti `WorkingTimeCollection`.

```csharp
public class WorkingTimeCollection : IList<WorkingTime>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Count](../../aspose.tasks/workingtimecollection/count/) { get; } | Ottiene il numero di oggetti contenuti in questo oggetto `WorkingTimeCollection`. |
| [Item](../../aspose.tasks/workingtimecollection/item/) { get; set; } | Restituisce l'elemento all'indice specificato. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.tasks/workingtimecollection/add/)(WorkingTime) | Aggiunge una nuova istanza di WorkingTime a questa collezione. |
| [Clear](../../aspose.tasks/workingtimecollection/clear/)() | Rimuove tutti gli elementi [`WorkingTime`](../workingtime/) dalla collezione. |
| [Contains](../../aspose.tasks/workingtimecollection/contains/)(WorkingTime) | Verifica se l'elemento specificato è nella Lista. Esegue una ricerca lineare O(n). |
| [CopyTo](../../aspose.tasks/workingtimecollection/copyto/)(WorkingTime[], int) | copia il contenuto di una collezione in un Array, iniziando da un indice specifico |
| [GetEnumerator](../../aspose.tasks/workingtimecollection/getenumerator/)() | Restituisce un enumeratore per questa collezione. |
| [Remove](../../aspose.tasks/workingtimecollection/remove/)(WorkingTime) | Rimuove l'istanza [`WorkingTime`](../workingtime/) da questa collezione. |
| [ToList](../../aspose.tasks/workingtimecollection/tolist/)() | Converte l'oggetto WorkingTimeCollection in una lista di oggetti [`WorkingTime`](../workingtime/). |

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

* class [WorkingTime](../workingtime/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


