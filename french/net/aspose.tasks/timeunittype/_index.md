---
title: "Enum TimeUnitType"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.TimeUnitType enum. Spécifie le type d'une unité de temps"
type: docs
weight: 2570
url: /fr/net/aspose.tasks/timeunittype/
---
## TimeUnitType enumeration

Spécifie le type d'une unité de temps.

```csharp
public enum TimeUnitType : sbyte
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Undefined | `-1` | Indique que la valeur Undefined signifie que le champ n'était pas défini dans le fichier de projet original. |
| Minute | `0` | Indique le type d'unité de temps Minute. |
| ElapsedMinute | `1` | Indique le type d'unité de temps minute écoulée. |
| Hour | `2` | Indique le type d'unité de temps Heure. |
| ElapsedHour | `3` | Indique le type d'unité de temps heure écoulée. |
| Day | `4` | Indique le type d'unité de temps Jour. |
| ElapsedDay | `5` | Indique le type d'unité de temps jour écoulé. |
| Week | `6` | Indique le type d'unité de temps Semaine. |
| ElapsedWeek | `7` | Indique le type d'unité de temps semaine écoulée. |
| Month | `8` | Indique le type d'unité de temps Mois. |
| ElapsedMonth | `9` | Indique le type d'unité de temps mois écoulé. |
| Percent | `10` | Indique le type d'unité de temps Pourcentage. |
| ElapsedPercent | `11` | Indique le type d'unité de temps pourcentage écoulé. |
| Null | `12` | Indique le type d'unité de temps Null. |
| MinuteEstimated | `13` | Indique le type d'unité de temps estimée Minute. |
| ElapsedMinuteEstimated | `14` | Indique le type d'unité de temps estimée minute écoulée. |
| HourEstimated | `15` | Indique le type d'unité de temps estimée Heure. |
| ElapsedHourEstimated | `16` | Indique le type d'unité de temps estimée heure écoulée. |
| DayEstimated | `17` | Indique le type d'unité de temps estimée Jour. |
| ElapsedDayEstimated | `18` | Indique le type d'unité de temps estimée jour écoulé. |
| WeekEstimated | `19` | Indique le type d'unité de temps estimée Semaine. |
| ElapsedWeekEstimated | `20` | Indique le type d'unité de temps estimée semaine écoulée. |
| MonthEstimated | `21` | Indique le type d'unité de temps estimée Mois. |
| ElapsedMonthEstimated | `22` | Indique le type d'unité de temps estimée mois écoulé. |
| PercentEstimated | `23` | Indique le type d'unité de temps estimée Pourcentage. |
| ElapsedPercentEstimated | `24` | Indique le type d'unité de temps estimé en pourcentage écoulé. |
| Year | `25` | Indique le type d'unité de temps Année. |

## Remarques

Lors de l'exportation vers XML, les valeurs Undefined seront éliminées du XML résultant.

## Exemples

Montre comment convertir une durée en différents types d'unités de temps.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// Obtenez une tâche pour calculer sa durée dans différents formats
var task = project.RootTask.Children.GetById(1);

// Obtenez la durée en Minutes, Jours, Heures, Semaines et Mois
var mins = task.Get(Tsk.Duration).Convert(TimeUnitType.Minute).ToDouble();
Console.WriteLine("Duration in Mins: {0}", mins);
var days = task.Get(Tsk.Duration).Convert(TimeUnitType.Day).ToDouble();
Console.WriteLine("Duration in Days: {0}", days);
var hours = task.Get(Tsk.Duration).Convert(TimeUnitType.Hour).ToDouble();
Console.WriteLine("Duration in Hours: {0}", hours);
var weeks = task.Get(Tsk.Duration).Convert(TimeUnitType.Week).ToDouble();
Console.WriteLine("Duration in Weeks: {0}", weeks);
var months = task.Get(Tsk.Duration).Convert(TimeUnitType.Month).ToDouble();
Console.WriteLine("Duration in Months: {0}", months);
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


