---
title: "Calendar.GetIntersectionCalendar"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Calendar. Получает экземпляр ICalendar, который можно использовать для выполнения вычислений пересечения графиков работы двух календарей"
type: docs
weight: 280
url: /ru/net/aspose.tasks/calendar/getintersectioncalendar/
---
## Calendar.GetIntersectionCalendar method

Получает экземпляр [`ICalendar`](../../icalendar/), который можно использовать для выполнения вычислений пересечения графиков работы двух календарей.

```csharp
public static ICalendar GetIntersectionCalendar(Calendar calendar1, Calendar calendar2)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| calendar1 | Calendar | Первый календарь. |
| calendar2 | Calendar | Второй календарь. |

### Возвращаемое значение

Реализация интерфейса ICalendar.

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException | Когда любой из аргументов равен null. |

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

* interface [ICalendar](../../icalendar/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


