---
title: "CalendarCollection.GetEnumerator"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод CalendarCollection. Возвращает перечислитель для этой коллекции"
type: docs
weight: 50
url: /ru/net/aspose.tasks/calendarcollection/getenumerator/
---
## CalendarCollection.GetEnumerator method

Возвращает перечислитель для этой коллекции.

```csharp
public IEnumerator<Calendar> GetEnumerator()
```

### Возвращаемое значение

перечислитель для этой коллекции.

## Примеры

Показывает, как добавить новые календари.

```csharp
var project = new Project();

// Новые календари могут быть добавлены в коллекцию календарей проекта с помощью перегрузок метода Add коллекции.
project.Calendars.Add("Calendar");
var newCalendar = project.Calendars.Add("Parent");
project.Calendars.Add("Child", newCalendar);

foreach (var calendar in project.Calendars)
{
    Console.WriteLine("Calendar Name: " + calendar.Name);
}
```

### См. также

* class [Calendar](../../calendar/)
* class [CalendarCollection](../)
* namespace [Aspose.Tasks](../../calendarcollection/)
* assembly [Aspose.Tasks](../../../)


