---
title: Class CalendarException
second_title: Référence de l'API Aspose.Tasks pour .NET
description: Aspose.Tasks.CalendarException classe. Représenter des périodes exceptionnelles dans un calendrier.
type: docs
weight: 250
url: /fr/net/aspose.tasks/calendarexception/
---
## CalendarException class

Représenter des périodes exceptionnelles dans un calendrier.

```csharp
public sealed class CalendarException
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [CalendarException](calendarexception/)() | Initialise une nouvelle instance du`CalendarException` classe. |

## Propriétés

| Nom | La description |
| --- | --- |
| [DaysOfWeek](../../aspose.tasks/calendarexception/daysofweek/) { get; } | Obtient la DayTypeCollection pour cet objet. Les jours de la semaine où l'exception est valide. |
| [DayWorking](../../aspose.tasks/calendarexception/dayworking/) { get; set; } | Obtient ou définit une valeur indiquant si la date ou le type de jour spécifié fonctionne. |
| [EnteredByOccurrences](../../aspose.tasks/calendarexception/enteredbyoccurrences/) { get; set; } | Obtient ou définit une valeur indiquant si la plage de récurrence est définie en saisissant un nombre d'occurrences. False spécifie que la plage de récurrence est définie en saisissant une date de fin. |
| [FromDate](../../aspose.tasks/calendarexception/fromdate/) { get; set; } | Obtient ou définit le début de l'heure d'exception. |
| [Month](../../aspose.tasks/calendarexception/month/) { get; set; } | Obtient ou définit le mois pour lequel une récurrence d'exception est planifiée. |
| [MonthDay](../../aspose.tasks/calendarexception/monthday/) { get; set; } | Obtient ou définit le jour d'un mois auquel une récurrence d'exception est planifiée. |
| [MonthItem](../../aspose.tasks/calendarexception/monthitem/) { get; set; } | Obtient ou définit l'élément du mois pour lequel une récurrence d'exception est planifiée. |
| [MonthPosition](../../aspose.tasks/calendarexception/monthposition/) { get; set; } | Obtient ou définit la position d'un élément de mois dans un mois. |
| [Name](../../aspose.tasks/calendarexception/name/) { get; set; } | Obtient ou définit le nom de l'exception. |
| [Occurrences](../../aspose.tasks/calendarexception/occurrences/) { get; set; } | Obtient ou définit le nombre d'occurrences pour lesquelles l'exception de calendrier est valide. |
| [ParentCalendar](../../aspose.tasks/calendarexception/parentcalendar/) { get; } | Obtient le calendrier parent de cet objet. |
| [Period](../../aspose.tasks/calendarexception/period/) { get; set; } | Obtient ou définit la période de récurrence de l'exception. |
| [ToDate](../../aspose.tasks/calendarexception/todate/) { get; set; } | Obtient ou définit la fin de l'heure d'exception. |
| [Type](../../aspose.tasks/calendarexception/type/) { get; set; } | Obtient ou définit le type d'exception. |
| [WorkingTimes](../../aspose.tasks/calendarexception/workingtimes/) { get; set; } | Obtient ou définit l'objet WorkingTimeCollection. La collection de temps de travail qui définit le temps travaillé le jour de la semaine.  Au moins un temps de travail doit être présent, et il ne peut y en avoir plus de cinq. |

## Méthodes

| Nom | La description |
| --- | --- |
| [CheckException](../../aspose.tasks/calendarexception/checkexception/)(DateTime) | Renvoie true si l'instance spécifiée duDateTime struct est le jour d'exception. |
| [Delete](../../aspose.tasks/calendarexception/delete/)() | Supprime l'instance d'exception de l'objet CalendarExceptionCollection du calendrier parent. |
| [GetExceptionDates](../../aspose.tasks/calendarexception/getexceptiondates/)() | Renvoie les dates auxquelles l'exception de calendrier est applicable. |
| [GetWorkingTime](../../aspose.tasks/calendarexception/getworkingtime/)() | Renvoie le temps de travail pour une exception de calendrier. |

### Voir également

* espace de noms [Aspose.Tasks](../../aspose.tasks/)
* Assemblée [Aspose.Tasks](../../)


