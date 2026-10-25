---
title: "CalendarException.EnteredByOccurrences"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété CalendarException. Obtient ou définit une valeur indiquant si la plage de récurrence est définie en saisissant un nombre d'occurrences. False indique que la plage de récurrence est définie en saisissant une date de fin."
type: docs
weight: 40
url: /fr/net/aspose.tasks/calendarexception/enteredbyoccurrences/
---
## CalendarException.EnteredByOccurrences property

Obtient ou définit une valeur indiquant si la plage de récurrence est définie en saisissant un nombre d'occurrences. False indique que la plage de récurrence est définie en saisissant une date de fin.

```csharp
public bool EnteredByOccurrences { get; set; }
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


