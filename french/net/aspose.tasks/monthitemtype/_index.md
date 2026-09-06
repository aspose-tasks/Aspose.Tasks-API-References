---
title: "Enum MonthItemType"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.MonthItemType enum. Spécifie l'élément de mois pour lequel une récurrence d'exception est planifiée."
type: docs
weight: 1050
url: /fr/net/aspose.tasks/monthitemtype/
---
## MonthItemType enumeration

Spécifie l'élément du mois pour lequel une récurrence d'exception est planifiée.

```csharp
public enum MonthItemType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Undefined | `-1` | Indique le type d'élément de mois Undefined. |
| Day | `0` | Indique le type d'élément de mois Day. |
| Weekday | `1` | Indique le type d'élément de mois Weekday. |
| WeekendDay | `2` | Indique le type d'élément de mois WeekendDay. |
| Sunday | `3` | Indique le type d'élément de mois Sunday. |
| Monday | `4` | Indique le type d'élément de mois Monday. |
| Tuesday | `5` | Indique le type d'élément de mois Tuesday. |
| Wednesday | `6` | Indique le type d'élément de mois Wednesday. |
| Thursday | `7` | Indique le type d'élément de mois Thursday. |
| Friday | `8` | Indique le type d'élément de mois Friday. |
| Saturday | `9` | Indique le type d'élément de mois Saturday. |

## Exemples

Montre comment définir une exception de calendrier par jour du mois.

```csharp
var project = new Project(DataDir + "project_test.mpp");

// créer un calendrier
var calendar = project.Calendars.Add("Calendar1");

// créer une exception de calendrier pour chaque vendredi
var exception = new CalendarException();
exception.Type = CalendarExceptionType.MonthlyByDay;
exception.FromDate = new DateTime(2010, 1, 1);
exception.ToDate = new DateTime(2020, 12, 31);
exception.Month = Month.December;
exception.MonthDay = 1;
exception.MonthItem = MonthItemType.Undefined;
exception.MonthPosition = MonthPosition.Last;
exception.Period = 5;

// vérifier qu'un vendredi est exceptionnel
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2012, 12, 1)));

// ajoutez l'exception au calendrier
calendar.Exceptions.Add(exception);
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


