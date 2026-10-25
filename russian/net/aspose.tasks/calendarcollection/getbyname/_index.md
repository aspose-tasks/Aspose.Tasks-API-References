---
title: "CalendarCollection.GetByName"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод CalendarCollection. Возвращает календарь с указанным именем"
type: docs
weight: 30
url: /ru/net/aspose.tasks/calendarcollection/getbyname/
---
## CalendarCollection.GetByName method

Возвращает календарь с указанным именем.

```csharp
public Calendar GetByName(string name)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | Строка | Имя календаря. |

### Возвращаемое значение

Если найден, возвращает календарь с указанным именем, иначе возвращает null.

## Примеры

Показывает, как получить календари по имени или по идентификатору.

```csharp
var project = new Project(DataDir + "Project5.mpp");

var calendarByName = project.Calendars.GetByName("TestCalendar");
var calendarByUid = project.Calendars.GetByUid(4);

Console.WriteLine("Calendar Name: " + calendarByName.Name);
Console.WriteLine("Calendar Name: " + calendarByUid.Name);
Console.WriteLine("Are calendars equals: " + calendarByName.Equals(calendarByUid));
```

### См. также

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


