---
title: "Énumération DayType"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Énumération Aspose.Tasks.DayType. Spécifie le jour d'une semaine"
type: docs
weight: 450
url: /fr/net/aspose.tasks/daytype/
---
## DayType enumeration

Spécifie le jour de la semaine.

```csharp
public enum DayType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Exception | `0` | Indique le type de jour Exception. |
| Sunday | `1` | Indique le type de jour Dimanche. |
| Monday | `2` | Indique le type de jour Lundi. |
| Tuesday | `3` | Indique le type de jour Mardi. |
| Wednesday | `4` | Indique le type de jour Mercredi. |
| Thursday | `5` | Indique le type de jour Jeudi. |
| Friday | `6` | Indique le type de jour Vendredi. |
| Saturday | `7` | Indique le type de jour Samedi. |

## Exemples

Montre comment définir un nouveau calendrier, y ajouter les jours de la semaine et définir les heures de travail pour les jours.

```csharp
var project = new Project();

// Définir un calendrier
var calendar = project.Calendars.Add("Calendar1");

// Ajouter les jours de travail du lundi au jeudi avec les horaires par défaut
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// Définir le vendredi comme jour de travail court
var weekDay = new WeekDay(DayType.Friday);

// Définit le temps de travail. Seule la partie heure de DateTime est importante
var workingTime = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 16);
weekDay.WorkingTimes.Add(workingTime);
weekDay.WorkingTimes.Add(workingTime2);
weekDay.DayWorking = true;
calendar.WeekDays.Add(weekDay);

// travail avec le projet...
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


