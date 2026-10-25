---
title: "Classe Calendar"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Calendar classe. Représente un calendrier utilisé dans un projet."
type: docs
weight: 230
url: /fr/net/aspose.tasks/calendar/
---
## Calendar class

Représente un calendrier utilisé dans un projet.

```csharp
public class Calendar : ICalendar
```

## Propriétés

| Nom | Description |
| --- | --- |
| [BaseCalendar](../../aspose.tasks/calendar/basecalendar/) { get; set; } | Obtient ou définit le calendrier de base dont dépend ce calendrier. Applicable uniquement si le calendrier n'est pas un calendrier de base. |
| [Exceptions](../../aspose.tasks/calendar/exceptions/) { get; } | Obtient l'objet CalendarExceptionCollection. La collection d'exceptions associée au calendrier. |
| [Guid](../../aspose.tasks/calendar/guid/) { get; } | Obtient le GUID du calendrier. |
| [IsBaseCalendar](../../aspose.tasks/calendar/isbasecalendar/) { get; } | Obtient une valeur indiquant si le calendrier est un calendrier de base. |
| [IsBaselineCalendar](../../aspose.tasks/calendar/isbaselinecalendar/) { get; set; } | Obtient ou définit une valeur indiquant si le calendrier est un calendrier de référence. |
| [Name](../../aspose.tasks/calendar/name/) { get; set; } | Obtient ou définit le nom du calendrier. |
| [PrimaveraProperties](../../aspose.tasks/calendar/primaveraproperties/) { get; } | Obtient un objet contenant les propriétés spécifiques à Primavera pour un calendrier lu à partir des formats Primavera. |
| [Uid](../../aspose.tasks/calendar/uid/) { get; set; } | Obtient ou définit l'identifiant unique du calendrier. |
| [WeekDays](../../aspose.tasks/calendar/weekdays/) { get; } | Obtient WeekDaysCollection pour ce calendrier. La collection des jours de la semaine qui définit le calendrier. |
| [WorkWeeks](../../aspose.tasks/calendar/workweeks/) { get; } | Obtient l'objet WorkWeekCollections. La collection des semaines de travail associée au calendrier. |

## Méthodes

| Nom | Description |
| --- | --- |
| static [Make24HourCalendar](../../aspose.tasks/calendar/make24hourcalendar/)(Calendar) | Transforme un calendrier donné en calendrier 24Heures. Le calendrier 24Heures est un calendrier dans lequel chaque jour de la semaine travaille avec des heures de travail 24/24. |
| static [MakeNightShiftCalendar](../../aspose.tasks/calendar/makenightshiftcalendar/)(Calendar) | Transforme un calendrier donné en calendrier de quart de nuit. |
| static [MakeStandardCalendar](../../aspose.tasks/calendar/makestandardcalendar/)(Calendar) | Crée un calendrier standard par défaut. |
| [Delete](../../aspose.tasks/calendar/delete/)() | Supprime le calendrier du projet. |
| override [Equals](../../aspose.tasks/calendar/equals/)(object) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork)(DateTime, Duration) | Calcule la date à laquelle la quantité spécifiée de temps de travail sera écoulée selon le calendrier. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork/#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | Calcule la date à laquelle la quantité spécifiée de temps de travail sera écoulée selon le calendrier. |
| override [GetHashCode](../../aspose.tasks/calendar/gethashcode/)() | Renvoie un code de hachage pour l'instance de la classe. |
| [GetNextWorkingDayStart](../../aspose.tasks/calendar/getnextworkingdaystart/)(DateTime) | Calcule le début du prochain jour ouvrable pour la date spécifiée. |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/calendar/getpreviousworkingdayend/)(DateTime) | Calcule la fin du jour ouvrable précédent à partir de la date spécifiée. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration)(DateTime, Duration) | Renvoie la date de début basée sur la date de fin et la durée spécifiées. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | Renvoie la date de début basée sur la date de fin et la durée spécifiées. |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/calendar/gettaskfinishdatefromduration/)(Task, TimeSpan) | Calcule la date et l'heure de fin de la tâche à partir de sa date de début, de ses parties séparées et de la durée du travail. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours_1)(DateTime) | Renvoie le nombre d'heures de travail à la date spécifiée. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours/#getworkinghours)(DateTime, DateTime) | Renvoie WorkUnit - Début, Fin et Durée des heures de travail pour l'intervalle de date et d'heure spécifié. |
| [GetWorkingHoursTimeSpan](../../aspose.tasks/calendar/getworkinghourstimespan/)(DateTime, DateTime) | Renvoie le nombre d'heures de travail entre les dates spécifiées. |
| [GetWorkingTimes](../../aspose.tasks/calendar/getworkingtimes/)(DateTime) | Renvoie [`WorkingTimeCollection`](../workingtimecollection/) des temps de travail pour la date spécifiée. |
| [GetWorkStart](../../aspose.tasks/calendar/getworkstart/)(DateTime) | Calcule le début du prochain temps de travail à partir de la date et de l'heure spécifiées. |
| [IsDayWorking](../../aspose.tasks/calendar/isdayworking/)(DateTime) | Détermine si le jour spécifié est un jour ouvrable selon le calendrier. |
| virtual [IsEmpty](../../aspose.tasks/calendar/isempty/)() | Renvoie si le calendrier n'a pas d'heures de travail définies. |
| static [GetIntersectionCalendar](../../aspose.tasks/calendar/getintersectioncalendar/)(Calendar, Calendar) | Obtient l'instance [`ICalendar`](../icalendar/) qui peut être utilisée pour effectuer des calculs sur l'intersection des horaires de travail de 2 calendriers. |

## Remarques

Les calendriers sont utilisés pour définir les périodes de travail et de non-travail standard. Les projets doivent disposer d'un calendrier de base. Les tâches et les ressources peuvent avoir leurs propres calendriers non de base qui sont basés sur un calendrier de base.

## Exemples

Comment créer un calendrier simple à partir de zéro.

```csharp
[C#]
// créer un calendrier vide
Calendar calendar = new Calendar("New calendar");
// ajoute les jours de travail par défaut (8 heures de travail de 9 h00 à 17 h00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
// créer un nouveau jour de travail
WeekDay myWeekDay = new WeekDay(DayType.Thursday);
// Définit le temps de travail. Seule la partie heure de DateTime est importante
    WorkingTime wt1 = new WorkingTime();
    wt1.FromTime = new DateTime(1, 1, 1, 6, 0, 0, 0);
    wt1.ToTime = new DateTime(1, 1, 1, 12, 0, 0, 0);
    WorkingTime wt2 = new WorkingTime();
    wt2.FromTime = new DateTime(1, 1, 1, 14, 0, 0, 0);
    wt2.ToTime = new DateTime(1, 1, 1, 18, 0, 0, 0);
    myWeekDay.WorkingTimes.Add(wt1);
    myWeekDay.WorkingTimes.Add(wt2);
    myWeekDay.DayWorking = true;
calendar.Days.Add(myWeekDay);
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));
// ajoute le week-end
calendar.Days.Add(new WeekDay(DayType.Saturday));
calendar.Days.Add(new WeekDay(DayType.Sunday));
```

```csharp
[VB]
' create empty calendar
Dim calendar As Calendar =  New Calendar("New calendar")
' adds default working days (8 working hours from 9:00 to 17:00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday))
' create new new working day
Dim myWeekDay As WeekDay =  New WeekDay(DayType.Thursday)
' Sets working time. Only time part of DateTime is important
    Dim wt1 As WorkingTime =  New WorkingTime()
    wt1.FromTime = New DateTime(1, 1, 1, 6, 0, 0, 0)
    wt1.ToTime = New DateTime(1, 1, 1, 12, 0, 0, 0)
    Dim wt2 As WorkingTime =  New WorkingTime()
    wt2.FromTime = New DateTime(1, 1, 1, 14, 0, 0, 0)
    wt2.ToTime = New DateTime(1, 1, 1, 18, 0, 0, 0)
    myWeekDay.WorkingTimes.Add(wt1)
    myWeekDay.WorkingTimes.Add(wt2)
    myWeekDay.DayWorking = True
calendar.Days.Add(myWeekDay)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday))
' adds weekend
calendar.Days.Add(New WeekDay(DayType.Saturday))
calendar.Days.Add(New WeekDay(DayType.Sunday))
```

Montre comment définir un nouveau calendrier, y ajouter les jours de la semaine et définir les heures de travail pour les jours.

```csharp
var project = new Project();

// Définir un calendrier
var calendar = project.Calendars.Add("Calendar1");

// Ajouter les jours de travail du lundi au jeudi avec les horaires par défaut
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// Définir le vendredi comme jour de travail court
var weekDay = new WeekDay(DayType.Friday);

// Définit le temps de travail. Seule la partie heure de DateTime est importante
var workingTime = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 16);
weekDay.WorkingTimes.Add(workingTime);
weekDay.WorkingTimes.Add(workingTime2);
weekDay.DayWorking = true;
calendar.WeekDays.Add(weekDay);

// travail avec le projet...
```

### Voir aussi

* interface [ICalendar](../icalendar/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


