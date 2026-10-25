---
title: "WeekDay.WeekDay"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Costruttore WeekDay. Inizializza una nuova istanza della classe WeekDay con il tipo di giorno specificato"
type: docs
weight: 10
url: /it/net/aspose.tasks/weekday/weekday/
---
## WeekDay(DayType) {#constructor_1}

Inizializza una nuova istanza della classe [`WeekDay`](../) con il tipo di giorno specificato.

```csharp
public WeekDay(DayType dayType)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dayType | DayType | Il tipo di giorno specificato. |

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

* enum [DayType](../../daytype/)
* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)

---

## WeekDay(DayType, IEnumerable&lt;WorkingTime&gt;) {#constructor_3}

Inizializza una nuova istanza della classe [`WeekDay`](../) con il tipo di giorno specificato e l'elenco dei periodi di orario di lavoro.

```csharp
public WeekDay(DayType dayType, IEnumerable<WorkingTime> workingTimes)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dayType | DayType | Il tipo di giorno specificato. |
| workingTimes | IEnumerable`1 | Elenco dei periodi di orario di lavoro. |

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

* enum [DayType](../../daytype/)
* class [WorkingTime](../../workingtime/)
* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)

---

## WeekDay(DayType, params WorkingTime[]) {#constructor_2}

Inizializza una nuova istanza della classe [`WeekDay`](../) con il tipo di giorno specificato e i periodi di orario di lavoro.

```csharp
public WeekDay(DayType dayType, params WorkingTime[] workingTimes)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dayType | DayType | Il tipo di giorno specificato. |
| workingTimes | WorkingTime[] | Array di periodi di orario di lavoro. |

### Vedi anche

* enum [DayType](../../daytype/)
* class [WorkingTime](../../workingtime/)
* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)

---

## WeekDay() {#constructor}

Inizializza una nuova istanza della classe [`WeekDay`](../).

```csharp
public WeekDay()
```

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

* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)


