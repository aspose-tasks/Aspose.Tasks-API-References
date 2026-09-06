---
title: "Énumération CalendarExceptionType"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Énumération Aspose.Tasks.CalendarExceptionType. Spécifie le type d'exception du calendrier"
type: docs
weight: 270
url: /fr/net/aspose.tasks/calendarexceptiontype/
---
## CalendarExceptionType enumeration

Spécifie le type d’exception du calendrier.

```csharp
public enum CalendarExceptionType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Daily | `0` | Indique le type d'exception quotidien. |
| YearlyByDay | `1` | Indique le type d'exception annuel par jour du mois. |
| YearlyByPosition | `2` | Indique le type d'exception annuel par position. |
| MonthlyByDay | `3` | Indique le type d'exception mensuel par jour du mois. |
| MonthlyByPosition | `4` | Indique le type d'exception mensuel par position. |
| Weekly | `5` | Indique le type d'exception hebdomadaire. |
| ByDayCount | `6` | Indique le type d'exception par nombre de jours. |
| ByWeekDayCount | `7` | Indique le type d'exception par nombre de jours de semaine. |
| NoExceptionType | `8` | Indique aucun type d'exception. |

## Exemples

Montre comment définir une exception de calendrier par occurrences.

```csharp
var project = new Project();

// Définir un calendrier
var calendar = project.Calendars.Add("Calendar1");

// Définir une exception et spécifier les occurrences
var exception = new CalendarException();
exception.EnteredByOccurrences = true;
exception.Occurrences = 5;
exception.Type = CalendarExceptionType.YearlyByDay;
exception.MonthDay = 22;
exception.Month = Month.April;

// Ajouter une exception au calendrier
calendar.Exceptions.Add(exception);
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


