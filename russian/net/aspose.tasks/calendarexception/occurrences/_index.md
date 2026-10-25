---
title: "CalendarException.Occurrences"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство CalendarException. Получает или задает количество повторений, для которых исключение календаря действительно"
type: docs
weight: 110
url: /ru/net/aspose.tasks/calendarexception/occurrences/
---
## CalendarException.Occurrences property

Получает или задает количество повторений, в течение которых исключение календаря действительно.

```csharp
public int Occurrences { get; set; }
```

## Примеры

Показывает, как определить исключение календаря по вхождениям.

```csharp
var project = new Project();

// Определить календарь
var calendar = project.Calendars.Add("Calendar1");

// Определите исключение и укажите вхождения
var exception = new CalendarException();
exception.EnteredByOccurrences = true;
exception.Occurrences = 5;
exception.Type = CalendarExceptionType.YearlyByDay;
exception.MonthDay = 22;
exception.Month = Month.April;

// Добавить исключение в календарь
calendar.Exceptions.Add(exception);
```

### См. также

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


