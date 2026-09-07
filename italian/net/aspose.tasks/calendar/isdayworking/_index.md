---
title: "Calendar.IsDayWorking"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Calendar method. Determina se il giorno specificato è un giorno lavorativo secondo il calendario"
type: docs
weight: 260
url: /it/net/aspose.tasks/calendar/isdayworking/
---
## Calendar.IsDayWorking method

Determina se il giorno specificato è un giorno lavorativo secondo il calendario.

```csharp
public bool IsDayWorking(DateTime dt)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| dt | DateTime | La data da verificare per capire se il giorno è lavorativo. |

### Valore di ritorno

Vero se il giorno è un giorno lavorativo.

## Esempi

Mostra come calcolare le ore lavorative.

```csharp
var project = new Project(DataDir + "CalculateWorkHours.mpp");

// Accedi al Task per ID
var task = project.RootTask.Children.GetById(1);

// Accedi al calendario e alle sue date di inizio e fine
var taskCalendar = task.Get(Tsk.Calendar);
var startDate = task.Get(Tsk.Start);
var endDate = task.Get(Tsk.Finish);

// Accedi alla risorsa e al suo calendario
var resource = project.Resources.GetByUid(1);
var resourceCalendar = resource.Get(Rsc.Calendar);

TimeSpan timeSpan;

// Ottieni la durata in minuti
double durationInMins = 0;
var tempDate = startDate;
while (tempDate < endDate)
{
    if (taskCalendar.IsDayWorking(tempDate) && resourceCalendar.IsDayWorking(tempDate))
    {
        timeSpan = taskCalendar.GetWorkingHours(tempDate);
        durationInMins += timeSpan.TotalMinutes;
    }

    tempDate = tempDate.AddDays(1);
}

tempDate = startDate;

// Ottieni la durata in ore
double durationInHours = 0;
while (tempDate < endDate)
{
    if (taskCalendar.IsDayWorking(tempDate) && resourceCalendar.IsDayWorking(tempDate))
    {
        timeSpan = taskCalendar.GetWorkingHours(tempDate);
        durationInHours += timeSpan.TotalHours;
    }

    tempDate = tempDate.AddDays(1);
}

// Ottieni la durata in giorni
double durationInDays = 0;
tempDate = startDate;
while (tempDate < endDate)
{
    if (taskCalendar.IsDayWorking(tempDate) && resourceCalendar.IsDayWorking(tempDate))
    {
        timeSpan = taskCalendar.GetWorkingHours(tempDate);
        if (timeSpan.TotalHours > 0)
        {
            durationInDays += timeSpan.TotalDays * (24 / timeSpan.TotalHours);
        }
    }

    tempDate = tempDate.AddDays(1);
}

Console.WriteLine("Duration in Minutes = " + durationInMins);
Console.WriteLine("Duration in Hours = " + durationInHours);
Console.WriteLine("Duration in Days = " + durationInDays);
```

### Vedi anche

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


