---
title: "Enum MonthPosition"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Enum Aspose.Tasks.MonthPosition. Spécifie la position d'un élément du mois au sein du mois"
type: docs
weight: 1070
url: /fr/net/aspose.tasks/monthposition/
---
## MonthPosition enumeration

Spécifie la position d'un élément du mois au sein d'un mois.

```csharp
public enum MonthPosition
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Undefined | `-1` | Indique une position de mois non définie. |
| First | `0` | Indique la première position du mois. |
| Second | `1` | Indique la deuxième position du mois. |
| Third | `2` | Indique la troisième position du mois. |
| Fourth | `3` | Indique la position du quatrième mois. |
| Last | `4` | Indique la position du dernier mois. |

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


