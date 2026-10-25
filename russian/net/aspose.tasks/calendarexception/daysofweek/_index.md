---
title: "CalendarException.DaysOfWeek"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство CalendarException. Получает DayTypeCollection для этого объекта. Дни недели, в которые исключение действительно"
type: docs
weight: 20
url: /ru/net/aspose.tasks/calendarexception/daysofweek/
---
## CalendarException.DaysOfWeek property

Возвращает DayTypeCollection для этого объекта. Дни недели, в которые исключение действительно.

```csharp
public DayTypeCollection DaysOfWeek { get; }
```

## Примеры

Показывает, как определить исключение календаря по дню недели.

```csharp
var project = new Project(DataDir + "project_test.mpp");

// создать календарь
var calendar = project.Calendars.Add("Calendar1");

// создать исключение календаря для каждой пятницы
var exception = new CalendarException();
exception.Type = CalendarExceptionType.Weekly;
exception.FromDate = new DateTime(2020, 4, 6);
exception.ToDate = new DateTime(2020, 4, 12);
exception.DaysOfWeek.Add(DayType.Friday);

// проверьте, что пятница является исключением
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2020, 4, 10)));

// добавьте исключение в календарь
calendar.Exceptions.Add(exception);
```

### См. также

* class [DayTypeCollection](../../daytypecollection/)
* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


