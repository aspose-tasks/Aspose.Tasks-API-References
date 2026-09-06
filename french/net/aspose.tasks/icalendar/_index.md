---
title: "Interface ICalendar"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Interface Aspose.Tasks.ICalendar. Représente une abstraction de calendrier pouvant être utilisée pour divers calculs de dates et de durées."
type: docs
weight: 840
url: /fr/net/aspose.tasks/icalendar/
---
## ICalendar interface

Représente une abstraction de calendrier qui peut être utilisée pour divers calculs de dates et de durées.

```csharp
public interface ICalendar
```

## Méthodes

| Nom | Description |
| --- | --- |
| [GetFinishDateByStartAndWork](../../aspose.tasks/icalendar/getfinishdatebystartandwork/#getfinishdatebystartandwork)(DateTime, Duration) | Calcule la date à laquelle la quantité spécifiée de temps de travail sera écoulée selon le calendrier. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/icalendar/getfinishdatebystartandwork/#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | Calcule la date à laquelle la quantité spécifiée de temps de travail sera écoulée selon le calendrier. |
| [GetNextWorkingDayStart](../../aspose.tasks/icalendar/getnextworkingdaystart/)(DateTime) | Calcule le début du prochain jour ouvrable pour la date spécifiée. |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/icalendar/getpreviousworkingdayend/)(DateTime) | Calcule la fin du jour ouvrable précédent à partir de la date spécifiée. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/icalendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration)(DateTime, Duration) | Renvoie la date de début basée sur la date de fin et la durée spécifiées. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/icalendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | Renvoie la date de début basée sur la date de fin et la durée spécifiées. |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/icalendar/gettaskfinishdatefromduration/)(Task, TimeSpan) | Calcule la date et l'heure de fin de la tâche à partir de sa date de début, de ses parties séparées et de la durée du travail. |
| [GetWorkingHours](../../aspose.tasks/icalendar/getworkinghours/#getworkinghours_1)(DateTime) | Renvoie le nombre d'heures de travail à la date spécifiée. |
| [GetWorkingHours](../../aspose.tasks/icalendar/getworkinghours/#getworkinghours)(DateTime, DateTime) | Renvoie WorkUnit - Début, Fin et Durée des heures de travail pour l'intervalle de date et d'heure spécifié. |
| [GetWorkingHoursTimeSpan](../../aspose.tasks/icalendar/getworkinghourstimespan/)(DateTime, DateTime) | Renvoie le nombre d'heures de travail entre les dates spécifiées. |
| [GetWorkingTimes](../../aspose.tasks/icalendar/getworkingtimes/)(DateTime) | Renvoie [`WorkingTimeCollection`](../workingtimecollection/) des temps de travail pour la date spécifiée. |
| [GetWorkStart](../../aspose.tasks/icalendar/getworkstart/)(DateTime) | Calcule le début du prochain temps de travail à partir de la date et de l'heure spécifiées. |
| [IsDayWorking](../../aspose.tasks/icalendar/isdayworking/)(DateTime) | Détermine si le jour spécifié est un jour ouvrable selon le calendrier. |
| [IsEmpty](../../aspose.tasks/icalendar/isempty/)() | Renvoie si le calendrier n'a pas d'heures de travail définies. |

## Exemples

Montre comment utiliser la méthode Calendar.GetIntersectionCalendar() pour effectuer le calcul sur le calendrier de l'affectation.

```csharp
var project = new Project(DataDir + "CalculateWorkHours.mpp");

foreach (var ra in project.ResourceAssignments)
{
    if (ra.Resource == null)
    {
        continue;
    }

    ICalendar assignmentCalendar;

    Calendar taskCalendar = ra.Task.Calendar != null && !ra.Task.Duration.IsEstimated ? ra.Task.Calendar : null;
    Calendar resourceCalendar = ra.Resource.Calendar != null && !ra.Task.IgnoreResourceCalendar
        ? ra.Resource.Calendar
        : null;

    if (taskCalendar != null && resourceCalendar != null && !ReferenceEquals(taskCalendar, resourceCalendar))
    {
        assignmentCalendar = Calendar.GetIntersectionCalendar(taskCalendar, resourceCalendar);
    }
    else
    {
        assignmentCalendar = taskCalendar ?? resourceCalendar;
    }

    if (assignmentCalendar == null)
    {
        assignmentCalendar = project.Calendar;
    }

    var workingHours = assignmentCalendar.GetWorkingHours(ra.Start, ra.Finish);

    Console.WriteLine("Working hours for assignment '{0}' : {1}", ra, workingHours);

    var date = new DateTime(2025, 4, 7);
    Console.WriteLine("Working times for date '{0}':", date);

    foreach (var wt in assignmentCalendar.GetWorkingTimes(date))
    {
        Console.WriteLine("{0} - {1}", wt.From.TimeOfDay, wt.To.TimeOfDay);
    }
}
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


