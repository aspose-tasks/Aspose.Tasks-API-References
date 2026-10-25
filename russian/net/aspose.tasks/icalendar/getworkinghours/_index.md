---
title: "ICalendar.GetWorkingHours"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ICalendar. Возвращает WorkUnit, начало, конец и продолжительность рабочих часов для указанного интервала даты и времени."
type: docs
weight: 60
url: /ru/net/aspose.tasks/icalendar/getworkinghours/
---
## GetWorkingHours(DateTime, DateTime) {#getworkinghours}

Возвращает WorkUnit — начало, завершение и длительность рабочих часов для указанного интервала даты и времени.

```csharp
public WorkUnit GetWorkingHours(DateTime start, DateTime finish)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| start | DateTime | Дата начала интервала. |
| завершение | DateTime | Дата завершения интервала. |

### Возвращаемое значение

Экземпляр класса [`WorkUnit`](../../workunit/), содержащий начало, конец и продолжительность рабочих часов.

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

* class [WorkUnit](../../workunit/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetWorkingHours(DateTime) {#getworkinghours_1}

Возвращает количество рабочих часов на указанную дату.

```csharp
public TimeSpan GetWorkingHours(DateTime dt)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| dt | DateTime | Дата, для которой нужно получить рабочие часы. |

### Возвращаемое значение

Рабочие часы на указанную дату.

### См. также

* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


