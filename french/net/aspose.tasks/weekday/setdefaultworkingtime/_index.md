---
title: "WeekDay.SetDefaultWorkingTime"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode WeekDay. Définit les périodes de temps par défaut pour le jour de la semaine spécifié"
type: docs
weight: 130
url: /fr/net/aspose.tasks/weekday/setdefaultworkingtime/
---
## WeekDay.SetDefaultWorkingTime method

Définit les périodes de temps par défaut pour le jour de la semaine spécifié.

```csharp
public static void SetDefaultWorkingTime(WeekDay day)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| jour | WeekDay | Le jour de la semaine sur lequel définir le jour de travail par défaut. |

## Exemples

Montre comment définir une heure de travail par défaut pour une journée.

```csharp
var project = new Project();

// Définir un calendrier
var calendar = project.Calendars.Add("Calendar1");
calendar.WeekDays.Clear();

// Ajouter les jours de travail du lundi au jeudi avec les horaires par défaut
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


