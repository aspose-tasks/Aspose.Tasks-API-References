---
title: "Calendar.IsDayWorking"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Calendar. Détermine si le jour spécifié est un jour ouvrable selon le calendrier"
type: docs
weight: 260
url: /fr/net/aspose.tasks/calendar/isdayworking/
---
## Calendar.IsDayWorking method

Détermine si le jour spécifié est un jour ouvrable selon le calendrier.

```csharp
public bool IsDayWorking(DateTime dt)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| dt | DateTime | La date à vérifier si le jour est ouvrable. |

### Valeur de retour

Vrai si le jour est ouvrable.

## Exemples

Montre comment calculer les heures de travail.

```csharp
var project = new Project(DataDir + "CalculateWorkHours.mpp");

// Accéder à la tâche par ID
var task = project.RootTask.Children.GetById(1);

// Accéder au calendrier et à ses dates de début et de fin
var taskCalendar = task.Get(Tsk.Calendar);
var startDate = task.Get(Tsk.Start);
var endDate = task.Get(Tsk.Finish);

// Accéder à la ressource et à son calendrier
var resource = project.Resources.GetByUid(1);
var resourceCalendar = resource.Get(Rsc.Calendar);

TimeSpan timeSpan;

// Obtenir la durée en minutes
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

// Obtenir la durée en heures
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

// Obtenir la durée en jours
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

### Voir aussi

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


