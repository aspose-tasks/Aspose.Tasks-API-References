---
title: "CalendarException.WorkingTimes"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство CalendarException. Получает или задает объект WorkingTimeCollection. Коллекция рабочих времён, определяющая время работы в будний день. Должно присутствовать как минимум одно рабочее время, и их не может быть более пяти."
type: docs
weight: 160
url: /ru/net/aspose.tasks/calendarexception/workingtimes/
---
## CalendarException.WorkingTimes property

Получает или задает объект WorkingTimeCollection. Коллекция рабочих времён, определяющая время работы в будний день. Должно присутствовать как минимум одно рабочее время, и их не может быть более пяти.

```csharp
public WorkingTimeCollection WorkingTimes { get; set; }
```

## Примеры

Показывает, как получить рабочее время исключения календаря.

```csharp
var project = new Project(DataDir + "CalendarExceptions.mpp");

var calendar = project.Calendars.ToList()[0];
var exception = calendar.Exceptions[0];

Console.WriteLine("Calendar Name: " + calendar.Name);
Console.WriteLine("Calendar Exception Count: " + calendar.Exceptions.Count);
Console.WriteLine("Calendar Exception Name: " + exception.Name);
Console.WriteLine();

var workingTime = exception.GetWorkingTime();
Console.WriteLine("Exception Working Time: " + workingTime);

foreach (var time in exception.WorkingTimes)
{
    Console.WriteLine("Working Time Start: " + time.From);
    Console.WriteLine("Working Time Finish: " + time.To);
}
```

### См. также

* class [WorkingTimeCollection](../../workingtimecollection/)
* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


