---
title: Calendar
second_title: Référence de l'API Aspose.Tasks pour .NET
description: Représente un calendrier utilisé dans un projet.
type: docs
weight: 220
url: /fr/net/aspose.tasks/calendar/
---
## Calendar class

Représente un calendrier utilisé dans un projet.

```csharp
public class Calendar
```

## Propriétés

| Nom | La description |
| --- | --- |
| [BaseCalendar](../../aspose.tasks/calendar/basecalendar) { get; set; } | Obtient ou définit le calendrier de base dont dépend ce calendrier. Applicable uniquement si le calendrier n'est pas un calendrier de base. Lecture/écriture[`Calendar`](../calendar) . |
| [Exceptions](../../aspose.tasks/calendar/exceptions) { get; } | Obtient l'objet CalendarExceptionCollection. La collection d'exceptions associée au calendrier. |
| [IsBaseCalendar](../../aspose.tasks/calendar/isbasecalendar) { get; } | Obtient une valeur indiquant si le calendrier est un calendrier de base. Lecture seuleBoolean . |
| [IsBaselineCalendar](../../aspose.tasks/calendar/isbaselinecalendar) { get; set; } | Obtient ou définit une valeur indiquant si le calendrier est un calendrier de base. Lecture/écritureBoolean . |
| [Name](../../aspose.tasks/calendar/name) { get; set; } | Obtient ou définit le nom du calendrier. Lecture/écritureString . |
| [ParentProject](../../aspose.tasks/calendar/parentproject) { get; } | Obtient le projet parent pour ce calendrier. |
| [Uid](../../aspose.tasks/calendar/uid) { get; set; } | Obtient ou définit l'identifiant unique du calendrier. Lecture/écritureInt32 . |
| [WeekDays](../../aspose.tasks/calendar/weekdays) { get; } | Obtient WeekDaysCollection pour ce calendrier. La collection de jours de la semaine qui définit le calendrier. |
| [WorkWeeks](../../aspose.tasks/calendar/workweeks) { get; } | Obtient l'objet WorkWeekCollections. La collection de semaines de travail associée au calendrier. |

## Méthodes

| Nom | La description |
| --- | --- |
| static [Make24HourCalendar](../../aspose.tasks/calendar/make24hourcalendar)(Calendar) | Transforme un calendrier donné en calendrier 24 heures. Le calendrier 24 heures est un calendrier dans lequel chaque jour de la semaine fonctionne avec des heures de travail 24 heures sur 24. |
| static [MakeNightShiftCalendar](../../aspose.tasks/calendar/makenightshiftcalendar)(Calendar) | Transforme un calendrier donné en calendrier de nuit. |
| static [MakeStandardCalendar](../../aspose.tasks/calendar/makestandardcalendar)(Calendar) | Crée un calendrier standard par défaut. |
| [Delete](../../aspose.tasks/calendar/delete)() | Supprime le calendrier du projet. |
| override [Equals](../../aspose.tasks/calendar/equals)(object) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork#getfinishdatebystartandwork)(DateTime, Duration) | Calcule la date à laquelle le temps de travail spécifié passera selon le calendrier. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/calendar/getfinishdatebystartandwork#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | Calcule la date à laquelle le temps de travail spécifié passera selon le calendrier. |
| override [GetHashCode](../../aspose.tasks/calendar/gethashcode)() | Renvoie un code de hachage pour l'instance du[`Calendar`](../calendar) classe. |
| [GetNextWorkingDayStart](../../aspose.tasks/calendar/getnextworkingdaystart)(DateTime) | Calcule le début du jour ouvrable suivant à partir de la date. |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/calendar/getpreviousworkingdayend)(DateTime) | Calcule la date de fin de travail précédente à partir de la date spécifiée. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration#getstartdatefromfinishandduration)(DateTime, Duration) | Renvoie la date de début en fonction de la date de fin et de la durée spécifiées. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/calendar/getstartdatefromfinishandduration#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | Renvoie la date de début en fonction de la date de fin et de la durée spécifiées. |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/calendar/gettaskfinishdatefromduration)(Task, TimeSpan) | Calcule la date et l'heure de fin de la tâche à partir de sa date de début, des parties fractionnées et de la durée. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours#getworkinghours_1)(DateTime) | Renvoie le nombre d'heures de travail à la date. |
| [GetWorkingHours](../../aspose.tasks/calendar/getworkinghours#getworkinghours)(DateTime, DateTime) | Renvoie les heures de travail pour les dates spécifiées. |
| [GetWorkingTimes](../../aspose.tasks/calendar/getworkingtimes)(DateTime) | Retours[`WorkingTimeCollection`](../workingtimecollection) des temps de travail. |
| [IsDayWorking](../../aspose.tasks/calendar/isdayworking)(DateTime) | Détermine si le jour est un jour ouvré. |

### Remarques

Les calendriers sont utilisés pour définir les périodes ouvrées et chômées standard. Les projets doivent avoir un calendrier de base. Les tâches et les ressources peuvent avoir leurs propres calendriers non basés sur un calendrier de base.

### Exemples

Comment créer un calendrier simple à partir de zéro.

```csharp
[C#]
// crée un calendrier vide
Calendar calendar = new Calendar("New calendar");
// ajoute des jours ouvrés par défaut (8 heures ouvrées de 9h00 à 17h00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
// crée un nouveau nouveau jour de travail
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
' créer un calendrier vide
Dim calendar As Calendar =  New Calendar("New calendar")
' ajoute des jours ouvrables par défaut (8 heures ouvrables de 9h00 à 17h00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday))
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday))
' créer un nouveau jour de travail
Dim myWeekDay As WeekDay =  New WeekDay(DayType.Thursday)
' Définit le temps de travail. Seule la partie heure de DateTime est importante
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
' ajoute le week-end
calendar.Days.Add(New WeekDay(DayType.Saturday))
calendar.Days.Add(New WeekDay(DayType.Sunday))
```

### Voir également

* espace de noms [Aspose.Tasks](../../aspose.tasks)
* Assemblée [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
