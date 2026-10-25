---
title: "Schnittstelle ICalendar"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "Aspose.Tasks.ICalendar Schnittstelle. Stellt eine Kalenderabstraktion dar, die für verschiedene Berechnungen von Daten und Zeitspannen verwendet werden kann"
type: docs
weight: 840
url: /de/net/aspose.tasks/icalendar/
---
## ICalendar interface

Stellt eine Kalenderabstraktion dar, die für verschiedene Berechnungen von Daten und Zeitspannen verwendet werden kann.

```csharp
public interface ICalendar
```

## Methoden

| Name | Beschreibung |
| --- | --- |
| [GetFinishDateByStartAndWork](../../aspose.tasks/icalendar/getfinishdatebystartandwork/#getfinishdatebystartandwork)(DateTime, Duration) | Berechnet das Datum, an dem die angegebene Arbeitszeit gemäß dem Kalender verstrichen ist. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/icalendar/getfinishdatebystartandwork/#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | Berechnet das Datum, an dem die angegebene Arbeitszeit gemäß dem Kalender verstrichen ist. |
| [GetNextWorkingDayStart](../../aspose.tasks/icalendar/getnextworkingdaystart/)(DateTime) | Berechnet den Beginn des nächsten Arbeitstages für das angegebene Datum. |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/icalendar/getpreviousworkingdayend/)(DateTime) | Berechnet das Ende des vorherigen Arbeitstages basierend auf dem angegebenen Datum. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/icalendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration)(DateTime, Duration) | Gibt das Startdatum basierend auf dem angegebenen Enddatum und der Dauer zurück. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/icalendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | Gibt das Startdatum basierend auf dem angegebenen Enddatum und der Dauer zurück. |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/icalendar/gettaskfinishdatefromduration/)(Task, TimeSpan) | Berechnet das Enddatum und die Endzeit einer Aufgabe aus ihrem Startdatum, den Teilabschnitten und der Arbeitsdauer. |
| [GetWorkingHours](../../aspose.tasks/icalendar/getworkinghours/#getworkinghours_1)(DateTime) | Gibt die Anzahl der Arbeitsstunden am angegebenen Datum zurück. |
| [GetWorkingHours](../../aspose.tasks/icalendar/getworkinghours/#getworkinghours)(DateTime, DateTime) | Gibt WorkUnit – Start, Ende und Dauer der Arbeitsstunden für das angegebene Datums‑Zeitintervall zurück. |
| [GetWorkingHoursTimeSpan](../../aspose.tasks/icalendar/getworkinghourstimespan/)(DateTime, DateTime) | Gibt die Anzahl der Arbeitsstunden zwischen den angegebenen Daten zurück. |
| [GetWorkingTimes](../../aspose.tasks/icalendar/getworkingtimes/)(DateTime) | Gibt [`WorkingTimeCollection`](../workingtimecollection/) der Arbeitszeiten für das angegebene Datum zurück. |
| [GetWorkStart](../../aspose.tasks/icalendar/getworkstart/)(DateTime) | Berechnet den Beginn der nächsten Arbeitszeit ab dem angegebenen Datum und der Uhrzeit. |
| [IsDayWorking](../../aspose.tasks/icalendar/isdayworking/)(DateTime) | Bestimmt, ob der angegebene Tag gemäß dem Kalender ein Arbeitstag ist. |
| [IsEmpty](../../aspose.tasks/icalendar/isempty/)() | Gibt zurück, ob der Kalender keine definierten Arbeitszeiten hat. |

## Beispiele

Zeigt, wie die Methode Calendar.GetIntersectionCalendar() verwendet wird, um Berechnungen im Kalender der Zuordnung durchzuführen.

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

### Siehe auch

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


