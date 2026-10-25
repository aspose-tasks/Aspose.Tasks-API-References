---
title: "CalendarException.EnteredByOccurrences"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство CalendarException. Получает или задает значение, указывающее, определяется ли диапазон повторения вводом количества повторений. False указывает, что диапазон повторения определяется вводом конечной даты"
type: docs
weight: 40
url: /ru/net/aspose.tasks/calendarexception/enteredbyoccurrences/
---
## CalendarException.EnteredByOccurrences property

Получает или задает значение, указывающее, определяется ли диапазон повторения вводом количества повторений. Значение False указывает, что диапазон повторения определяется вводом даты завершения.

```csharp
public bool EnteredByOccurrences { get; set; }
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


