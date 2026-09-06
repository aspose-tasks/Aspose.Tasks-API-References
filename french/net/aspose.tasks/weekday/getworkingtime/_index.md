---
title: "WeekDay.GetWorkingTime"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode WeekDay. Retourne le temps de travail pour un jour de la semaine"
type: docs
weight: 110
url: /fr/net/aspose.tasks/weekday/getworkingtime/
---
## WeekDay.GetWorkingTime method

Renvoie le temps de travail pour un jour de la semaine.

```csharp
public TimeSpan GetWorkingTime()
```

### Valeur de retour

Temps de travail.

## Exemples

Montre comment créer un nouveau calendrier en définissant les jours de la semaine.

```csharp
var project = new Project();

// Définir un calendrier
var calendar = project.Calendars.Add("Calendar1");

// Ajouter les jours de travail du lundi au jeudi avec les horaires par défaut
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(new WeekDay(DayType.Tuesday, new WorkingTime(9, 11), new WorkingTime(12, 18)));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));

var exceptionDay = WeekDay.CreateDefaultWorkingDay(DayType.Exception);
exceptionDay.FromDate = new DateTime(2020, 4, 27, 0, 0, 0);
exceptionDay.ToDate = new DateTime(2020, 4, 30, 0, 0, 0);
exceptionDay.DayWorking = false;
calendar.WeekDays.Add(exceptionDay);

// vérifier les dates de début et de fin du jour d’exception
Console.WriteLine("The from date is: " + exceptionDay.FromDate);
Console.WriteLine("The to date is: " + exceptionDay.ToDate);
Console.WriteLine();

calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// Définir le vendredi comme jour de travail court

// Définit le temps de travail. 
var workingTimes = new List<WorkingTime> { new WorkingTime(9, 12), new WorkingTime(13, 16) };

// il existe un moyen de convertir <see cref=\"DayOfWeek\" /> en <see cref=\"Aspose.Tasks.DayType\" />.
var dayType = WeekDay.CastToDayType(DayOfWeek.Friday);

var weekDay = new WeekDay(dayType, workingTimes);
weekDay.DayWorking = true;
Console.WriteLine("The day type is: " + weekDay.DayType);
Console.WriteLine("The from date is: " + weekDay.FromDate);
Console.WriteLine("The to date is: " + weekDay.ToDate);

calendar.WeekDays.Add(weekDay);

// lets print all working times
foreach (var day in calendar.WeekDays)
{
    Console.WriteLine("Day Type: " + day.DayType); 
    Console.WriteLine("Is working day: " + day.DayWorking); 
    Console.WriteLine("Working Time (Hours): " + day.GetWorkingTime().TotalHours);
    Console.WriteLine();
}
```

### Voir aussi

* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)


