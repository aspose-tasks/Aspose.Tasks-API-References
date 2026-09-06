---
title: "Classe WeekDay"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.WeekDay. Représente un jour de la semaine qui définit soit des jours réguliers d’une semaine, soit des jours d’exception dans un calendrier"
type: docs
weight: 3540
url: /fr/net/aspose.tasks/weekday/
---
## WeekDay class

Représente un jour de la semaine qui définit soit des jours réguliers d'une semaine, soit des jours d'exception dans un calendrier.

```csharp
public class WeekDay
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [WeekDay](weekday/#constructor)() | Initialise une nouvelle instance de la classe `WeekDay`. |
| [WeekDay](weekday/#constructor_1)(DayType) | Initialise une nouvelle instance de la classe `WeekDay` avec le type de jour spécifié. |
| [WeekDay](weekday/#constructor_3)(DayType, IEnumerable&lt;WorkingTime&gt;) | Initialise une nouvelle instance de la classe `WeekDay` avec le type de jour spécifié et la liste des périodes de travail. |
| [WeekDay](weekday/#constructor_2)(DayType, params WorkingTime[]) | Initialise une nouvelle instance de la classe `WeekDay` avec le type de jour spécifié et les périodes de travail. |

## Propriétés

| Nom | Description |
| --- | --- |
| [DayType](../../aspose.tasks/weekday/daytype/) { get; } | Obtient le type d’un jour. |
| [DayWorking](../../aspose.tasks/weekday/dayworking/) { get; set; } | Obtient ou définit une valeur indiquant si la date ou le type de jour spécifié est travaillé. |
| [FromDate](../../aspose.tasks/weekday/fromdate/) { get; set; } | Obtient ou définit le début d’une période d’exception. |
| [ToDate](../../aspose.tasks/weekday/todate/) { get; set; } | Obtient ou définit la fin d’une période d’exception. |
| [WorkingTimes](../../aspose.tasks/weekday/workingtimes/) { get; } | Obtient WorkingTimeCollection pour cette instance WeekDay. La collection des temps de travail qui définissent le temps travaillé sur le jour de la semaine. |

## Méthodes

| Nom | Description |
| --- | --- |
| static [CreateDefaultWorkingDay](../../aspose.tasks/weekday/createdefaultworkingday/)(DayType) | Crée un jour de travail par défaut. |
| [Clone](../../aspose.tasks/weekday/clone/)() | Renvoie une copie profonde du jour de la semaine. |
| override [Equals](../../aspose.tasks/weekday/equals/)(object) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| override [GetHashCode](../../aspose.tasks/weekday/gethashcode/)() | Renvoie une valeur de code de hachage pour l’instance de la classe `WeekDay`. |
| [GetWorkingTime](../../aspose.tasks/weekday/getworkingtime/)() | Renvoie le temps de travail pour un jour de la semaine. |
| static [CastToDayType](../../aspose.tasks/weekday/casttodaytype/)(DayOfWeek) | Convertit le DayOfWeek de .Net en [`DayType`](./daytype/). |
| static [SetDefaultWorkingTime](../../aspose.tasks/weekday/setdefaultworkingtime/)(WeekDay) | Définit les périodes de temps par défaut pour le jour de la semaine spécifié. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


