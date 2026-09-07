---
title: "Interfaccia ICalendar"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Interfaccia Aspose.Tasks.ICalendar. Rappresenta un'astrazione del calendario che può essere utilizzata per vari calcoli di date e durate."
type: docs
weight: 840
url: /it/net/aspose.tasks/icalendar/
---
## ICalendar interface

Rappresenta un'astrazione del calendario che può essere utilizzata per vari calcoli di date e durate.

```csharp
public interface ICalendar
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetFinishDateByStartAndWork](../../aspose.tasks/icalendar/getfinishdatebystartandwork/#getfinishdatebystartandwork)(DateTime, Duration) | Calcola la data in cui il tempo di lavoro specificato sarà trascorso secondo il calendario. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/icalendar/getfinishdatebystartandwork/#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | Calcola la data in cui il tempo di lavoro specificato sarà trascorso secondo il calendario. |
| [GetNextWorkingDayStart](../../aspose.tasks/icalendar/getnextworkingdaystart/)(DateTime) | Calcola l'inizio del prossimo giorno lavorativo per la data specificata. |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/icalendar/getpreviousworkingdayend/)(DateTime) | Calcola la fine della data lavorativa precedente a partire dalla data specificata. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/icalendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration)(DateTime, Duration) | Restituisce la data di inizio basata sulla data di fine e sulla durata specificate. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/icalendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | Restituisce la data di inizio basata sulla data di fine e sulla durata specificate. |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/icalendar/gettaskfinishdatefromduration/)(Task, TimeSpan) | Calcola la data e l'ora di fine dell'attività a partire dalla sua data di inizio, dalle parti suddivise e dalla durata del lavoro. |
| [GetWorkingHours](../../aspose.tasks/icalendar/getworkinghours/#getworkinghours_1)(DateTime) | Restituisce la quantità di ore lavorative nella data specificata. |
| [GetWorkingHours](../../aspose.tasks/icalendar/getworkinghours/#getworkinghours)(DateTime, DateTime) | Restituisce WorkUnit - Inizio, Fine e Durata delle ore lavorative per l'intervallo di data e ora specificato. |
| [GetWorkingHoursTimeSpan](../../aspose.tasks/icalendar/getworkinghourstimespan/)(DateTime, DateTime) | Restituisce la quantità di ore lavorative tra le date specificate. |
| [GetWorkingTimes](../../aspose.tasks/icalendar/getworkingtimes/)(DateTime) | Restituisce [`WorkingTimeCollection`](../workingtimecollection/) di orari di lavoro per la data specificata. |
| [GetWorkStart](../../aspose.tasks/icalendar/getworkstart/)(DateTime) | Calcola l'inizio del prossimo orario lavorativo a partire dalla data e ora specificate. |
| [IsDayWorking](../../aspose.tasks/icalendar/isdayworking/)(DateTime) | Determina se il giorno specificato è un giorno lavorativo secondo il calendario. |
| [IsEmpty](../../aspose.tasks/icalendar/isempty/)() | Restituisce se il calendario non ha ore lavorative definite. |

## Esempi

Mostra come utilizzare il metodo Calendar.GetIntersectionCalendar() per eseguire il calcolo sul calendario dell'assegnazione.

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

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


