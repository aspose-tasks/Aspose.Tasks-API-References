---
title: "CalendarException.Delete"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод CalendarException. Удаляет экземпляр Exception из родительского объекта CalendarExceptionCollection календаря"
type: docs
weight: 180
url: /ru/net/aspose.tasks/calendarexception/delete/
---
## CalendarException.Delete method

Удаляет экземпляр Exception из родительского объекта календаря CalendarExceptionCollection.

```csharp
public void Delete()
```

## Примеры

Показывает, как удалить исключение календаря.

```csharp
var project = new Project(DataDir + "CalendarExceptions.mpp");

var calendar = project.Calendars.ToList()[0];

Console.WriteLine("Calendar Name: " + calendar.Name);
Console.WriteLine("Calendar Exception Count: " + calendar.Exceptions.Count);

// удалить исключение
calendar.Exceptions[0].Delete();

Console.WriteLine("Calendar Exception Count: " + calendar.Exceptions.Count);
```

### См. также

* class [CalendarException](../)
* namespace [Aspose.Tasks](../../calendarexception/)
* assembly [Aspose.Tasks](../../../)


