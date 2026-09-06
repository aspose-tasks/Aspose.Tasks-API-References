---
title: "Classe CalendarException"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.CalendarException. Représente des périodes de temps exceptionnelles dans un calendrier"
type: docs
weight: 250
url: /fr/net/aspose.tasks/calendarexception/
---
## CalendarException class

Représente des périodes de temps exceptionnelles dans un calendrier.

```csharp
public sealed class CalendarException
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [CalendarException](calendarexception/)() | Initialise une nouvelle instance de la classe `CalendarException`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [DaysOfWeek](../../aspose.tasks/calendarexception/daysofweek/) { get; } | Obtient la DayTypeCollection pour cet objet. Les jours de la semaine pendant lesquels l'exception est valide. |
| [DayWorking](../../aspose.tasks/calendarexception/dayworking/) { get; set; } | Obtient ou définit une valeur indiquant si la date ou le type de jour spécifié est travaillé. |
| [EnteredByOccurrences](../../aspose.tasks/calendarexception/enteredbyoccurrences/) { get; set; } | Obtient ou définit une valeur indiquant si la plage de récurrence est définie en saisissant un nombre d'occurrences. False indique que la plage de récurrence est définie en saisissant une date de fin. |
| [FromDate](../../aspose.tasks/calendarexception/fromdate/) { get; set; } | Obtient ou définit le début de la période d'exception. |
| [Month](../../aspose.tasks/calendarexception/month/) { get; set; } | Obtient ou définit le mois pour lequel une récurrence d'exception est planifiée. |
| [MonthDay](../../aspose.tasks/calendarexception/monthday/) { get; set; } | Obtient ou définit le jour du mois auquel une récurrence d'exception est planifiée. |
| [MonthItem](../../aspose.tasks/calendarexception/monthitem/) { get; set; } | Obtient ou définit l'élément du mois pour lequel une récurrence d'exception est planifiée. |
| [MonthPosition](../../aspose.tasks/calendarexception/monthposition/) { get; set; } | Obtient ou définit la position d'un élément du mois au sein d'un mois. |
| [Name](../../aspose.tasks/calendarexception/name/) { get; set; } | Obtient ou définit le nom de l'exception. |
| [Occurrences](../../aspose.tasks/calendarexception/occurrences/) { get; set; } | Obtient ou définit le nombre d'occurrences pendant lesquelles l'exception de calendrier est valide. |
| [ParentCalendar](../../aspose.tasks/calendarexception/parentcalendar/) { get; } | Obtient le calendrier parent de cet objet. |
| [Period](../../aspose.tasks/calendarexception/period/) { get; set; } | Obtient ou définit la période de récurrence de l'exception. |
| [ToDate](../../aspose.tasks/calendarexception/todate/) { get; set; } | Obtient ou définit la fin de la période d'exception. |
| [Type](../../aspose.tasks/calendarexception/type/) { get; set; } | Obtient ou définit le type d'exception. |
| [WorkingTimes](../../aspose.tasks/calendarexception/workingtimes/) { get; set; } | Obtient ou définit l'objet WorkingTimeCollection. La collection des temps de travail qui définit le temps travaillé pendant la semaine. Au moins un temps de travail doit être présent, et il ne peut pas y en avoir plus de cinq. |

## Méthodes

| Nom | Description |
| --- | --- |
| [CheckException](../../aspose.tasks/calendarexception/checkexception/)(DateTime) | Renvoie true si l'instance spécifiée de la structure DateTime est le jour d'exception. |
| [Delete](../../aspose.tasks/calendarexception/delete/)() | Supprime l'instance Exception de l'objet calendrier parent CalendarExceptionCollection. |
| [GetExceptionDates](../../aspose.tasks/calendarexception/getexceptiondates/)() | Renvoie les dates auxquelles l'exception de calendrier s'applique. |
| [GetWorkingTime](../../aspose.tasks/calendarexception/getworkingtime/)() | Renvoie le temps de travail pour une exception de calendrier. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


