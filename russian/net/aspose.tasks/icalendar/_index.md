---
title: "Интерфейс ICalendar"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Интерфейс Aspose.Tasks.ICalendar. Представляет абстракцию календаря, которую можно использовать для различных вычислений дат и длительностей."
type: docs
weight: 840
url: /ru/net/aspose.tasks/icalendar/
---
## ICalendar interface

Представляет абстракцию календаря, которую можно использовать для различных вычислений дат и длительностей.

```csharp
public interface ICalendar
```

## Методы

| Имя | Описание |
| --- | --- |
| [GetFinishDateByStartAndWork](../../aspose.tasks/icalendar/getfinishdatebystartandwork/#getfinishdatebystartandwork)(DateTime, Duration) | Вычисляет дату, когда указанное количество рабочего времени пройдет согласно календарю. |
| [GetFinishDateByStartAndWork](../../aspose.tasks/icalendar/getfinishdatebystartandwork/#getfinishdatebystartandwork_1)(DateTime, TimeSpan) | Вычисляет дату, когда указанное количество рабочего времени пройдет согласно календарю. |
| [GetNextWorkingDayStart](../../aspose.tasks/icalendar/getnextworkingdaystart/)(DateTime) | Вычисляет начало следующего рабочего дня для указанной даты. |
| [GetPreviousWorkingDayEnd](../../aspose.tasks/icalendar/getpreviousworkingdayend/)(DateTime) | Вычисляет конец предыдущего рабочего дня относительно указанной даты. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/icalendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration)(DateTime, Duration) | Возвращает дату начала, исходя из указанной даты завершения и длительности. |
| [GetStartDateFromFinishAndDuration](../../aspose.tasks/icalendar/getstartdatefromfinishandduration/#getstartdatefromfinishandduration_1)(DateTime, TimeSpan) | Возвращает дату начала, исходя из указанной даты завершения и длительности. |
| [GetTaskFinishDateFromDuration](../../aspose.tasks/icalendar/gettaskfinishdatefromduration/)(Task, TimeSpan) | Вычисляет дату и время завершения задачи на основе её даты начала, разбитых частей и длительности работы. |
| [GetWorkingHours](../../aspose.tasks/icalendar/getworkinghours/#getworkinghours_1)(DateTime) | Возвращает количество рабочих часов на указанную дату. |
| [GetWorkingHours](../../aspose.tasks/icalendar/getworkinghours/#getworkinghours)(DateTime, DateTime) | Возвращает WorkUnit — начало, завершение и длительность рабочих часов для указанного интервала даты и времени. |
| [GetWorkingHoursTimeSpan](../../aspose.tasks/icalendar/getworkinghourstimespan/)(DateTime, DateTime) | Возвращает количество рабочих часов между указанными датами. |
| [GetWorkingTimes](../../aspose.tasks/icalendar/getworkingtimes/)(DateTime) | Возвращает [`WorkingTimeCollection`](../workingtimecollection/) рабочих периодов для указанной даты. |
| [GetWorkStart](../../aspose.tasks/icalendar/getworkstart/)(DateTime) | Вычисляет начало следующего рабочего периода, начиная с указанной даты и времени. |
| [IsDayWorking](../../aspose.tasks/icalendar/isdayworking/)(DateTime) | Определяет, является ли указанный день рабочим согласно календарю. |
| [IsEmpty](../../aspose.tasks/icalendar/isempty/)() | Возвращает, определено ли в календаре отсутствие рабочих часов. |

## Примеры

Показывает, как использовать метод Calendar.GetIntersectionCalendar() для выполнения расчётов в календаре назначения.

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

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


