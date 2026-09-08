---
title: "Класс CalendarCollection"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.CalendarCollection. Представляет коллекцию объектов Calendar."
type: docs
weight: 240
url: /ru/net/aspose.tasks/calendarcollection/
---
## CalendarCollection class

Представляет коллекцию объектов [`Calendar`](../calendar/).

```csharp
public class CalendarCollection : IList<Calendar>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Count](../../aspose.tasks/calendarcollection/count/) { get; } | Получает количество объектов, содержащихся в этом объекте `CalendarCollection`. |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.tasks/calendarcollection/add/#add)(string) | Добавляет новый базовый календарь в этот объект CalendarCollection и возвращает добавленный календарь. |
| [Add](../../aspose.tasks/calendarcollection/add/#add_1)(string, Calendar) | Добавляет новый календарь с указанным базовым календарем в этот объект CalendarCollection и возвращает добавленный календарь. |
| [GetByName](../../aspose.tasks/calendarcollection/getbyname/)(string) | Возвращает календарь с указанным именем. |
| [GetByUid](../../aspose.tasks/calendarcollection/getbyuid/)(int) | Возвращает календарь с указанным UID. |
| [GetEnumerator](../../aspose.tasks/calendarcollection/getenumerator/)() | Возвращает перечислитель для этой коллекции. |
| [Remove](../../aspose.tasks/calendarcollection/remove/)(Calendar) | Удаляет Calendar из Project CalendarCollection. |
| [ToList](../../aspose.tasks/calendarcollection/tolist/)() | Преобразует объект CalendarCollection в список объектов [`Calendar`](../calendar/). |

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

* class [Calendar](../calendar/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


