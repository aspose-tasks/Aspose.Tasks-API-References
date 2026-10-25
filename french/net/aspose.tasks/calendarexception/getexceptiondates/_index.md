---
title: "CalendarException.GetExceptionDates"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "CalendarException méthode. Retourne les dates auxquelles l'exception de calendrier s'applique"
type: docs
weight: 190
url: /fr/net/aspose.tasks/calendarexception/getexceptiondates/
---
## CalendarException.GetExceptionDates method

Renvoie les dates auxquelles l'exception de calendrier s'applique.

```csharp
public IEnumerable<DateTime> GetExceptionDates()
```

### Valeur de retour

Retourne une collection de dates d'exception pour lesquelles l'exception de calendrier s'applique.

## Exemples

Montre comment obtenir les dates pour lesquelles une exception de calendrier spécifique est effective.

```csharp
Project project = new Project(DataDir + "CalendarExceptions.mpp");
Calendar calendar = project.Calendars.GetByUid(1);
CalendarException calendarException = calendar.Exceptions[0];

foreach (var date in calendarException.GetExceptionDates())
{
    Console.WriteLine(date);
}
```

### Voir aussi

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


