---
title: "Interface ICalendar"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.ICalendar interface. Vertegenwoordigt een kalenderabstractie die kan worden gebruikt voor verschillende berekeningen van datums en duur."
type: docs
weight: 840
url: /nl/net/aspose.tasks/icalendar/
---
## ICalendar interface

Stelt een kalenderabstractie voor die kan worden gebruikt voor verschillende berekeningen van datums en duur.

```csharp
public interface ICalendar
```

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [GetFinishDateByStartAndWork](../../aspose.tasks/icalendar/getfinishdatebystartandwork/#getfinishdatebystartandwork)(DateTime, Duration) | Berekent de datum waarop de opgegeven hoeveelheid werktijd volgens de kalender zal verstrijken. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/icalendar/getfinishdatebystartandwork/#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | Berekent de datum waarop de opgegeven hoeveelheid werktijd volgens de kalender zal verstrijken. |
| [GetNextWorkingDayStart](../../aspose.tasks/icalendar/getnextworkingdaystart/)(DateTime) | Berekent het begin van de volgende werkdag voor de opgegeven datum. |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/icalendar/getpreviousworkingdayend/)(DateTime) | Berekent het einde van de vorige werkdag vanaf de opgegeven datum. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/icalendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration)(DateTime, Duration) | Retourneert de startdatum op basis van de opgegeven einddatum en duur. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/icalendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | Retourneert de startdatum op basis van de opgegeven einddatum en duur. |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/icalendar/gettaskfinishdatefromduration/)(Task, TimeSpan) | Berekent de einddatum en -tijd van de taak op basis van de startdatum, gesplitste delen en de werktijdduur. |
| [GetWorkingHours](../../aspose.tasks/icalendar/getworkinghours/#getworkinghours_1)(DateTime) | Retourneert het aantal werkuren op de opgegeven datum. |
| [GetWorkingHours](../../aspose.tasks/icalendar/getworkinghours/#getworkinghours)(DateTime, DateTime) | Retourneert WorkUnit - Start, Eind en Duur van werkuren voor het opgegeven datum-tijdinterval. |
| [GetWorkingHoursTimeSpan](../../aspose.tasks/icalendar/getworkinghourstimespan/)(DateTime, DateTime) | Retourneert het aantal werkuren tussen de opgegeven datums. |
| [GetWorkingTimes](../../aspose.tasks/icalendar/getworkingtimes/)(DateTime) | Retourneert [`WorkingTimeCollection`](../workingtimecollection/) van werktijden voor de opgegeven datum. |
| [GetWorkStart](../../aspose.tasks/icalendar/getworkstart/)(DateTime) | Berekent het begin van de volgende werktijd vanaf de opgegeven datum en tijd. |
| [IsDayWorking](../../aspose.tasks/icalendar/isdayworking/)(DateTime) | Bepaalt of de opgegeven dag een werkdag is volgens de kalender. |
| [IsEmpty](../../aspose.tasks/icalendar/isempty/)() | Retourneert of de kalender geen werkuren heeft gedefinieerd. |

## Voorbeelden

Toont hoe de methode Calendar.GetIntersectionCalendar() te gebruiken om berekeningen uit te voeren op de kalender van de toewijzing.

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

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


