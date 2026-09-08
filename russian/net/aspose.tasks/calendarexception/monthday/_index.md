---
title: "CalendarException.MonthDay"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство CalendarException. Получает или задает день месяца, в который запланировано повторение исключения"
type: docs
weight: 70
url: /ru/net/aspose.tasks/calendarexception/monthday/
---
## CalendarException.MonthDay property

Получает или задает день месяца, в который запланировано повторение исключения.

```csharp
public int MonthDay { get; set; }
```

## Примеры

Показывает, как определить исключение календаря по дню месяца.

```csharp
var project = new Project(DataDir + "project_test.mpp");

// создать календарь
var calendar = project.Calendars.Add("Calendar1");

// создать исключение календаря для каждой пятницы
var exception = new CalendarException();
exception.Type = CalendarExceptionType.MonthlyByDay;
exception.FromDate = new DateTime(2010, 1, 1);
exception.ToDate = new DateTime(2020, 12, 31);
exception.Month = Month.December;
exception.MonthDay = 1;
exception.MonthItem = MonthItemType.Undefined;
exception.MonthPosition = MonthPosition.Last;
exception.Period = 5;

// проверьте, что пятница является исключительной
Console.WriteLine("Is date an exception date: " + exception.CheckException(new DateTime(2012, 12, 1)));

// добавьте исключение в календарь
calendar.Exceptions.Add(exception);
```

### См. также

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


