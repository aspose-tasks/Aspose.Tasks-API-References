---
title: "CalendarCollection.Count"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство CalendarCollection. Возвращает количество объектов, содержащихся в этом объекте CalendarCollection"
type: docs
weight: 10
url: /ru/net/aspose.tasks/calendarcollection/count/
---
## CalendarCollection.Count property

Возвращает количество объектов, содержащихся в этом объекте [`CalendarCollection`](../).

```csharp
public int Count { get; }
```

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

* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


