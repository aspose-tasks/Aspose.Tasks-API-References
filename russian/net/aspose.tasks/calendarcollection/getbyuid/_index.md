---
title: "CalendarCollection.GetByUid"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод CalendarCollection. Возвращает календарь с указанным UID"
type: docs
weight: 40
url: /ru/net/aspose.tasks/calendarcollection/getbyuid/
---
## CalendarCollection.GetByUid method

Возвращает календарь с указанным UID.

```csharp
public Calendar GetByUid(int uid)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| uid | Int32 | UID календаря. |

### Возвращаемое значение

Календарь с указанным UID.

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


