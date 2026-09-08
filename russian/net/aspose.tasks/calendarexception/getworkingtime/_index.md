---
title: "CalendarException.GetWorkingTime"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод CalendarException. Возвращает рабочее время для исключения календаря."
type: docs
weight: 200
url: /ru/net/aspose.tasks/calendarexception/getworkingtime/
---
## CalendarException.GetWorkingTime method

Возвращает рабочее время для исключения календаря.

```csharp
public TimeSpan GetWorkingTime()
```

### Возвращаемое значение

Возвращает рабочее время для этого исключения календаря.

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

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


