---
title: "Calendar.IsDayWorking"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Calendar methode. Bepaalt of de opgegeven dag een werkdag is volgens de agenda"
type: docs
weight: 260
url: /nl/net/aspose.tasks/calendar/isdayworking/
---
## Calendar.IsDayWorking method

Bepaalt of de opgegeven dag een werkdag is volgens de kalender.

```csharp
public bool IsDayWorking(DateTime dt)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| dt | DateTime | De datum om te controleren of de dag een werkdag is. |

### Retourwaarde

Waar als de dag een werkdag is.

## Voorbeelden

Toont hoe werkuren te berekenen.

```csharp
var project = new Project(DataDir + "CalculateWorkHours.mpp");

// Taak openen op ID
var task = project.RootTask.Children.GetById(1);

// Toegang tot Calendar en de start- en einddatums
var taskCalendar = task.Get(Tsk.Calendar);
var startDate = task.Get(Tsk.Start);
var endDate = task.Get(Tsk.Finish);

// Toegang tot resource en hun agenda
var resource = project.Resources.GetByUid(1);
var resourceCalendar = resource.Get(Rsc.Calendar);

TimeSpan timeSpan;

// Duur in minuten ophalen
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

// Duur in uren ophalen
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

// Duur in dagen ophalen
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

### Zie ook

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


