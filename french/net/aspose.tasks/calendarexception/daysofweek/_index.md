---
title: "CalendarException.DaysOfWeek"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "CalendarException propriété. Obtient le DayTypeCollection pour cet objet. Les jours de la semaine pendant lesquels l'exception est valide."
type: docs
weight: 20
url: /fr/net/aspose.tasks/calendarexception/daysofweek/
---
## CalendarException.DaysOfWeek property

Obtient la DayTypeCollection pour cet objet. Les jours de la semaine pendant lesquels l'exception est valide.

```csharp
public DayTypeCollection DaysOfWeek { get; }
```

## Exemples

Montre comment définir une exception de calendrier par jour de la semaine.

```csharp
var project = new Project(DataDir + "project_test.mpp");

// créer un calendrier
var calendar = project.Calendars.Add("Calendar1");

// créer une exception de calendrier pour chaque vendredi
var exception = new CalendarException();
exception.Type = CalendarExceptionType.Weekly;
exception.FromDate = new DateTime(2020, 4, 6);
exception.ToDate = new DateTime(2020, 4, 12);
exception.DaysOfWeek.Add(DayType.Friday);

// vérifiez que vendredi est exceptionnel
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2020, 4, 10)));

// ajoutez l'exception au calendrier
calendar.Exceptions.Add(exception);
```

### Voir aussi

* class [DayTypeCollection](../../daytypecollection/)
* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


