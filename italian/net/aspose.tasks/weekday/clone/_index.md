---
title: "WeekDay.Clone"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo WeekDay. Restituisce una copia profonda del giorno della settimana"
type: docs
weight: 80
url: /it/net/aspose.tasks/weekday/clone/
---
## WeekDay.Clone method

Restituisce una copia profonda del giorno della settimana.

```csharp
public WeekDay Clone()
```

### Valore di ritorno

Restituisce la copia profonda del giorno della settimana.

## Esempi

Mostra come clonare un giorno della settimana.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var calendar = project.Calendars.GetByUid(1);
var weekDay1 = calendar.WeekDays[0];

// crea una copia profonda di un giorno della settimana
var weekDay2 = weekDay1.Clone();

// l'uguaglianza dei calendari viene verificata rispetto alle proprietà del giorno della settimana:
// weekday.DayType
// weekday.DayWorking
// weekday.FromDate
// weekday.ToDate
// weekday.WorkingTimes
Console.WriteLine("WeekDay 1 Day Type: " + weekDay1.DayType);
Console.WriteLine("WeekDay 1 Day Working: " + weekDay1.DayWorking);
Console.WriteLine("WeekDay 1 From Date: " + weekDay1.FromDate);
Console.WriteLine("WeekDay 1 From Date: " + weekDay1.ToDate);
Console.WriteLine("WeekDay 1 WorkingTimes: " + weekDay1.WorkingTimes);
Console.WriteLine("WeekDay 2 Day Type: " + weekDay2.DayType);
Console.WriteLine("WeekDay 2 Day Working: " + weekDay2.DayWorking);
Console.WriteLine("WeekDay 2 From Date: " + weekDay2.FromDate);
Console.WriteLine("WeekDay 2 From Date: " + weekDay2.ToDate);
Console.WriteLine("WeekDay 2 WorkingTimes: " + weekDay2.WorkingTimes);
Console.WriteLine("Are weekdays equal: " + weekDay1.Equals(weekDay2));
Console.WriteLine("Are weekdays equal (by reference): " + ReferenceEquals(weekDay1, weekDay2));
```

### Vedi anche

* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)


