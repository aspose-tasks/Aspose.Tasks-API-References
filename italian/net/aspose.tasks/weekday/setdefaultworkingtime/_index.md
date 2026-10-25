---
title: "WeekDay.SetDefaultWorkingTime"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "WeekDay metodo. Imposta i periodi di tempo predefiniti per il giorno della settimana specificato"
type: docs
weight: 130
url: /it/net/aspose.tasks/weekday/setdefaultworkingtime/
---
## WeekDay.SetDefaultWorkingTime method

Imposta i periodi di tempo predefiniti per il giorno della settimana specificato.

```csharp
public static void SetDefaultWorkingTime(WeekDay day)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| giorno | WeekDay | Il giorno della settimana su cui impostare il giorno lavorativo predefinito. |

## Esempi

Mostra come impostare un orario di lavoro predefinito per un giorno.

```csharp
var project = new Project();

// Definisci un calendario
var calendar = project.Calendars.Add("Calendar1");
calendar.WeekDays.Clear();

// Aggiungi giorni lavorativi da lunedì a giovedì con gli orari predefiniti
var monday = new WeekDay(DayType.Monday);
WeekDay.SetDefaultWorkingTime(monday);
calendar.WeekDays.Add(monday);
var tuesday = new WeekDay(DayType.Tuesday);
WeekDay.SetDefaultWorkingTime(tuesday);
calendar.WeekDays.Add(tuesday);
var wednesday = new WeekDay(DayType.Wednesday);
WeekDay.SetDefaultWorkingTime(wednesday);
calendar.WeekDays.Add(wednesday);
var thursday = new WeekDay(DayType.Thursday);
WeekDay.SetDefaultWorkingTime(thursday);
calendar.WeekDays.Add(thursday);
var friday = new WeekDay(DayType.Friday);
WeekDay.SetDefaultWorkingTime(friday);
calendar.WeekDays.Add(friday);

var saturday = new WeekDay(DayType.Saturday);
saturday.DayWorking = false;
calendar.WeekDays.Add(saturday);
var sunday = new WeekDay(DayType.Sunday);
sunday.DayWorking = false;
calendar.WeekDays.Add(sunday);

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


