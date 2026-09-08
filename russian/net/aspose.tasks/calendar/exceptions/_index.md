---
title: "Calendar.Exceptions"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Calendar. Возвращает объект CalendarExceptionCollection. Коллекция исключений, связанных с календарём."
type: docs
weight: 50
url: /ru/net/aspose.tasks/calendar/exceptions/
---
## Calendar.Exceptions property

Получает объект CalendarExceptionCollection. Коллекция исключений, связанных с календарем.

```csharp
public CalendarExceptionCollection Exceptions { get; }
```

## Примеры

Показывает, как получить информацию об исключениях календаря.

```csharp
var project = new Project(DataDir + "project_RetrieveExceptions_test.mpp");

// Перебрать календари
foreach (var calendar in project.Calendars)
{
    // Доступ к исключениям календаря
    foreach (var exception in calendar.Exceptions)
    {
        Console.WriteLine("From: " + exception.FromDate.ToShortDateString());
        Console.WriteLine("To: " + exception.ToDate.ToShortDateString());
    }
}
```

### См. также

* class [CalendarExceptionCollection](../../calendarexceptioncollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


