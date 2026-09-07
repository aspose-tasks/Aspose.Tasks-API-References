---
title: "Classe WeekDay"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.WeekDay. Rappresenta un giorno della settimana che definisce sia i giorni regolari di una settimana sia i giorni di eccezione in un calendario"
type: docs
weight: 3540
url: /it/net/aspose.tasks/weekday/
---
## WeekDay class

Rappresenta un giorno della settimana che definisce sia i giorni regolari di una settimana sia i giorni di eccezione in un calendario.

```csharp
public class WeekDay
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [WeekDay](weekday/#constructor)() | Inizializza una nuova istanza della classe `WeekDay`. |
| [WeekDay](weekday/#constructor_1)(DayType) | Inizializza una nuova istanza della classe `WeekDay` con il tipo di giorno specificato. |
| [WeekDay](weekday/#constructor_3)(DayType, IEnumerable&lt;WorkingTime&gt;) | Inizializza una nuova istanza della classe `WeekDay` con il tipo di giorno specificato e l'elenco dei periodi di tempo lavorativi. |
| [WeekDay](weekday/#constructor_2)(DayType, params WorkingTime[]) | Inizializza una nuova istanza della classe `WeekDay` con il tipo di giorno specificato e i periodi di tempo lavorativi. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [DayType](../../aspose.tasks/weekday/daytype/) { get; } | Ottiene il tipo di un giorno. |
| [DayWorking](../../aspose.tasks/weekday/dayworking/) { get; set; } | Ottiene o imposta un valore che indica se la data o il tipo di giorno specificato è lavorativo. |
| [FromDate](../../aspose.tasks/weekday/fromdate/) { get; set; } | Ottiene o imposta l'inizio di un periodo di eccezione. |
| [ToDate](../../aspose.tasks/weekday/todate/) { get; set; } | Ottiene o imposta la fine di un periodo di eccezione. |
| [WorkingTimes](../../aspose.tasks/weekday/workingtimes/) { get; } | Ottiene WorkingTimeCollection per questa istanza di WeekDay. La collezione di tempi di lavoro che definiscono il tempo lavorato nel giorno della settimana. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [CreateDefaultWorkingDay](../../aspose.tasks/weekday/createdefaultworkingday/)(DayType) | Crea un giorno lavorativo predefinito. |
| [Clone](../../aspose.tasks/weekday/clone/)() | Restituisce una copia profonda del giorno della settimana. |
| override [Equals](../../aspose.tasks/weekday/equals/)(object) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| override [GetHashCode](../../aspose.tasks/weekday/gethashcode/)() | Restituisce un valore di codice hash per l'istanza della classe `WeekDay`. |
| [GetWorkingTime](../../aspose.tasks/weekday/getworkingtime/)() | Restituisce il tempo di lavoro per un giorno della settimana. |
| static [CastToDayType](../../aspose.tasks/weekday/casttodaytype/)(DayOfWeek) | Converte DayOfWeek di .Net in [`DayType`](./daytype/). |
| static [SetDefaultWorkingTime](../../aspose.tasks/weekday/setdefaultworkingtime/)(WeekDay) | Imposta i periodi di tempo predefiniti per il giorno della settimana specificato. |

## Esempi

Mostra come creare un nuovo calendario definendo i giorni della settimana.

```csharp
var project = new Project();

// Definisci un calendario
var calendar = project.Calendars.Add("Calendar1");

// Aggiungi giorni lavorativi da lunedì a giovedì con gli orari predefiniti
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(new WeekDay(DayType.Tuesday, new WorkingTime(9, 11), new WorkingTime(12, 18)));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));

var exceptionDay = WeekDay.CreateDefaultWorkingDay(DayType.Exception);
exceptionDay.FromDate = new DateTime(2020, 4, 27, 0, 0, 0);
exceptionDay.ToDate = new DateTime(2020, 4, 30, 0, 0, 0);
exceptionDay.DayWorking = false;
calendar.WeekDays.Add(exceptionDay);

// verifica le date di inizio e fine del giorno di eccezione
Console.WriteLine("The from date is: " + exceptionDay.FromDate);
Console.WriteLine("The to date is: " + exceptionDay.ToDate);
Console.WriteLine();

calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// Imposta il venerdì come giorno lavorativo breve

// Imposta il tempo di lavoro. 
var workingTimes = new List<WorkingTime> { new WorkingTime(9, 12), new WorkingTime(13, 16) };

// esiste un modo per convertire <see cref=\"DayOfWeek\" /> in <see cref=\"Aspose.Tasks.DayType\" />.
var dayType = WeekDay.CastToDayType(DayOfWeek.Friday);

var weekDay = new WeekDay(dayType, workingTimes);
weekDay.DayWorking = true;
Console.WriteLine("The day type is: " + weekDay.DayType);
Console.WriteLine("The from date is: " + weekDay.FromDate);
Console.WriteLine("The to date is: " + weekDay.ToDate);

calendar.WeekDays.Add(weekDay);

// stampiamo tutti i tempi di lavoro
foreach (var day in calendar.WeekDays)
{
    Console.WriteLine("Day Type: " + day.DayType); 
    Console.WriteLine("Is working day: " + day.DayWorking); 
    Console.WriteLine("Working Time (Hours): " + day.GetWorkingTime().TotalHours);
    Console.WriteLine();
}
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


