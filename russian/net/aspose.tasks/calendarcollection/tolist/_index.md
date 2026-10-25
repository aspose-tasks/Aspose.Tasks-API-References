---
title: "CalendarCollection.ToList"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод CalendarCollection. Преобразует объект CalendarCollection в список объектов Calendar"
type: docs
weight: 70
url: /ru/net/aspose.tasks/calendarcollection/tolist/
---
## CalendarCollection.ToList method

Преобразует объект CalendarCollection в список объектов [`Calendar`](../../calendar/).

```csharp
public List<Calendar> ToList()
```

### Возвращаемое значение

Список объектов [`Calendar`](../../calendar/).

## Примеры

Показывает, как перебрать коллекцию календарей.

```csharp
var project = new Project(DataDir + "Project5.mpp");

Console.WriteLine("Number of calendars in the project: " + project.Calendars.Count);
List<Calendar> calendars = project.Calendars.ToList();
foreach (var calendar in calendars)
{
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### См. также

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


