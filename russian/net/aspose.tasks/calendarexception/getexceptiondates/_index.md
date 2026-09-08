---
title: "CalendarException.GetExceptionDates"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод CalendarException. Возвращает даты, на которые применяется исключение календаря"
type: docs
weight: 190
url: /ru/net/aspose.tasks/calendarexception/getexceptiondates/
---
## CalendarException.GetExceptionDates method

Возвращает даты, на которые применяется исключение календаря.

```csharp
public IEnumerable<DateTime> GetExceptionDates()
```

### Возвращаемое значение

Возвращает коллекцию дат-исключений, для которых применимо данное исключение календаря.

## Примеры

Показывает, как получить даты, для которых конкретное исключение календаря действительно.

```csharp
Project project = new Project(DataDir + "CalendarExceptions.mpp");
Calendar calendar = project.Calendars.GetByUid(1);
CalendarException calendarException = calendar.Exceptions[0];

foreach (var date in calendarException.GetExceptionDates())
{
    Console.WriteLine(date);
}
```

### См. также

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


