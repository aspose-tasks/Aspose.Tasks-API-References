---
title: "CalendarException.Period"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété CalendarException. Obtient ou définit la période de récurrence pour l'exception."
type: docs
weight: 130
url: /fr/net/aspose.tasks/calendarexception/period/
---
## CalendarException.Period property

Obtient ou définit la période de récurrence de l'exception.

```csharp
public int Period { get; set; }
```

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

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


