---
title: "CalendarException.Occurrences"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "CalendarException propriété. Obtient ou définit le nombre d'occurrences pour lesquelles l'exception de calendrier est valide."
type: docs
weight: 110
url: /fr/net/aspose.tasks/calendarexception/occurrences/
---
## CalendarException.Occurrences property

Obtient ou définit le nombre d'occurrences pendant lesquelles l'exception de calendrier est valide.

```csharp
public int Occurrences { get; set; }
```

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

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


