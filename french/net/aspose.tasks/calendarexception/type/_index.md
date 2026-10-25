---
title: "CalendarException.Type"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété CalendarException. Obtient ou définit le type d'exception."
type: docs
weight: 150
url: /fr/net/aspose.tasks/calendarexception/type/
---
## CalendarException.Type property

Obtient ou définit le type d'exception.

```csharp
public CalendarExceptionType Type { get; set; }
```

## Exemples

Montre comment ajouter/supprimer des exceptions de calendrier.

```csharp
var project = new Project(DataDir + "project_test.mpp");

// créer un calendrier
var calendar = project.Calendars.Add("Calendar1");

// crée une exception de jours de semaine pour un jour férié
var exception = new CalendarException();
exception.Name = "New Calendar Exception";
exception.EnteredByOccurrences = false;
exception.FromDate = new DateTime(2009, 12, 24, 0, 0, 0);
exception.ToDate = new DateTime(2009, 12, 31, 23, 59, 0);
exception.Type = CalendarExceptionType.Daily;
exception.Month = Month.December;

exception.DayWorking = false;

// vérifie que la date est exceptionnelle
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2009, 12, 26, 8, 0, 0)));

calendar.Exceptions.Add(exception);

// supprime une exception
var cal = project.Calendars.ToList()[0];
if (cal.Exceptions.Count > 1)
{
    var excToRemove = cal.Exceptions[0];
    cal.Exceptions.Remove(excToRemove);
}

// ajoute une exception
var exception2 = new CalendarException();
exception2.FromDate = new System.DateTime(2009, 1, 1);
exception2.ToDate = new System.DateTime(2009, 1, 3);
cal.Exceptions.Add(exception2);

// affiche les exceptions
foreach (var exc in cal.Exceptions)
{
    Console.WriteLine("Name: " + exc.Name);
    Console.WriteLine("From: " + exc.FromDate.ToShortDateString());
    Console.WriteLine("To: " + exc.ToDate.ToShortDateString());
}
```

### Voir aussi

* enum [CalendarExceptionType](../../calendarexceptiontype/)
* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


