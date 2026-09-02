---
title: "Aspose::Tasks::Calendar classe"
linktitle: "Calendrier"
articleTitle: "Calendrier"
second_title: "Aspose.Tasks pour C++"
description: "Représente un calendrier utilisé dans un projet."
type: docs
weight: 10
url: /fr/cpp/aspose.tasks/calendar/
---

## Calendar class

**Inherits:** Aspose::Tasks::ICalendar

Représente un calendrier utilisé dans un projet.

Comment créer un calendrier simple à partir de zéro.

```cpp
[C#]
// créer un calendrier vide
Calendar calendar = new Calendar("New calendar");
// ajoute les jours ouvrés par défaut (8 heures de travail de 9 h00 à 17 h00)
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.Days.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
// créer un nouveau jour ouvré
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

```cpp
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

Les calendriers sont utilisés pour définir les périodes de travail et de non‑travail standard. Les projets doivent disposer d'un calendrier de base. Les tâches et les ressources peuvent avoir leurs propres calendriers non de base qui sont basés sur un calendrier de base.

## Méthodes

| Nom | Description |
| --- | --- |
| [Delete](./delete/) | Supprime le calendrier du projet. |
| [Equals](./equals/) | Renvoie une valeur indiquant si cette instance est égale à un objet spécifié. |
| [get_BaseCalendar](./get_basecalendar/) | Obtient le calendrier de base dont dépend ce calendrier. Applicable uniquement si le calendrier n'est pas un calendrier de base. |
| [get_Exceptions](./get_exceptions/) | Obtient l'objet CalendarExceptionCollection. La collection d'exceptions associée au calendrier. |
| [get_Guid](./get_guid/) | Obtient le GUID du calendrier. |
| [get_IsBaseCalendar](./get_isbasecalendar/) | Obtient une valeur indiquant si le calendrier est un calendrier de base. |
| [get_IsBaselineCalendar](./get_isbaselinecalendar/) | Obtient une valeur indiquant si le calendrier est un calendrier de référence. |
| [get_Name](./get_name/) | Obtient le nom du calendrier. |
| [get_Uid](./get_uid/) | Obtient l'identifiant unique du calendrier. |
| [get_WeekDays](./get_weekdays/) | Obtient WeekDaysCollection pour ce calendrier. La collection des jours de la semaine qui définit le calendrier. |
| [get_WorkWeeks](./get_workweeks/) | Obtient l'objet WorkWeekCollections. La collection des semaines de travail associée au calendrier. |
| [GetFinishDateByStartAndWork (2 overloads)](./getfinishdatebystartandwork/) | Calcule la date à laquelle la quantité spécifiée de temps de travail sera écoulée selon le calendrier. |
| [GetHashCode](./gethashcode/) | Renvoie un code de hachage pour l'instance de la classe. |
| [GetIntersectionCalendar](./getintersectioncalendar/) | Obtient l'instance ICalendar qui peut être utilisée pour effectuer des calculs sur l'intersection des horaires de travail de 2 calendriers. |
| [GetNextWorkingDayStart](./getnextworkingdaystart/) | Calcule le début du prochain jour ouvrable pour la date spécifiée. |
| [GetPreviousWorkingDayEnd](./getpreviousworkingdayend/) | Calcule la fin du jour ouvrable précédent à partir de la date spécifiée. |
| [GetStartDateFromFinishAndDuration (2 overloads)](./getstartdatefromfinishandduration/) | Renvoie la date de début basée sur la date de fin et la durée spécifiées. |
| [GetTaskFinishDateFromDuration](./gettaskfinishdatefromduration/) | Calcule la date et l'heure de fin de la tâche à partir de sa date de début, de ses parties séparées et de la durée de travail. |
| [GetWorkingHours (2 overloads)](./getworkinghours/) | Renvoie le nombre d'heures de travail à la date spécifiée. |
| [GetWorkingHoursTimeSpan](./getworkinghourstimespan/) | Renvoie le nombre d'heures de travail entre les dates spécifiées. |
| [GetWorkingTimes](./getworkingtimes/) | Renvoie WorkingTimeCollection des temps de travail pour la date spécifiée. |
| [GetWorkStart](./getworkstart/) | Calcule le début du prochain temps de travail à partir de la date et de l'heure spécifiées. |
| [IsDayWorking](./isdayworking/) | Détermine si le jour spécifié est un jour ouvrable selon le calendrier. |
| [IsEmpty](./isempty/) | Renvoie si le calendrier n'a pas d'heures de travail définies. |
| [Make24HourCalendar](./make24hourcalendar/) | Transforme un calendrier donné en 24Hour Calendar. 24Hour Calendar est un calendrier dans lequel chaque jour de la semaine travaille avec des heures de travail continues. |
| [MakeNightShiftCalendar](./makenightshiftcalendar/) | Transforme un calendrier donné en Night Shift Calendar. |
| [MakeStandardCalendar](./makestandardcalendar/) | Crée un calendrier standard par défaut. |
| [set_BaseCalendar](./set_basecalendar/) | Définit le calendrier de base dont dépend ce calendrier. Applicable uniquement si le calendrier n'est pas un calendrier de base. |
| [set_IsBaselineCalendar](./set_isbaselinecalendar/) | Définit une valeur indiquant si le calendrier est un calendrier de référence. |
| [set_Name](./set_name/) | Définit le nom du calendrier. |
| [set_Uid](./set_uid/) | Définit l'identifiant unique du calendrier. |

