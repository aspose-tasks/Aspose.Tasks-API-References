---
title: "DayTypeCollection.Contains"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "DayTypeCollection метод. Возвращает true, если указанный элемент найден в этой коллекции, иначе false"
type: docs
weight: 60
url: /ru/net/aspose.tasks/daytypecollection/contains/
---
## DayTypeCollection.Contains method

Возвращает true, если указанный элемент найден в этой коллекции; в противном случае — false.

```csharp
public bool Contains(DayType item)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| элемент | DayType | указанный элемент для поиска. |

### Возвращаемое значение

true, если указанный элемент найден в этой коллекции; иначе false.

## Примеры

Показывает, как использовать коллекцию дней недели для определения исключения в недельном календаре.

```csharp
var project = new Project(DataDir + "WeeklyDayTypeException.mpp");
var calendar = project.Calendars.GetByUid(1);

foreach (var calendarException in calendar.Exceptions)
{
    Console.WriteLine("Exception Name: " + calendarException.Name);
    Console.WriteLine("Days of week count: " + calendarException.DaysOfWeek.Count);
    foreach (var dayType in calendarException.DaysOfWeek)
    {
        Console.WriteLine("Day type: " + dayType);
    }

    Console.WriteLine();
}

var exc1 = calendar.Exceptions.ToList()[0];
if (!exc1.DaysOfWeek.IsReadOnly && exc1.DaysOfWeek.IndexOf(DayType.Monday) < 0)
{
    exc1.DaysOfWeek.Insert(0, DayType.Wednesday);
}

var exc2 = calendar.Exceptions.ToList()[1];
if (exc2.DaysOfWeek.Contains(DayType.Sunday))
{
    // удалить тип дня из \"Exception 2\" по типу дня
    exc2.DaysOfWeek.Remove(DayType.Sunday);
}

// удалить тип дня из \"Exception 2\" по индексу
Console.WriteLine("Remove " + exc2.DaysOfWeek[0] + " day type from exception by index...");
exc2.DaysOfWeek.RemoveAt(0);

// Изменить исключения (в начальных данных проекта нет исключений)
var exc4 = new CalendarException
               {
                   Name = "Weekly Exception 2",
                   FromDate = new DateTime(2020, 4, 13),
                   ToDate = new DateTime(2020, 4, 18),
                   Occurrences = 3,
                   Type = CalendarExceptionType.Weekly
               };
exc4.DaysOfWeek.Add(DayType.Monday);
exc4.DaysOfWeek.Add(DayType.Thursday);

calendar.Exceptions.Add(exc4);

var exc3 = calendar.Exceptions.ToList()[2];

// удалить все дни недели для \"Exception 3\"
exc3.DaysOfWeek.Clear();

var dayTypes = new DayType[exc4.DaysOfWeek.Count];
exc4.DaysOfWeek.CopyTo(dayTypes, 0);

foreach (var dayType in dayTypes)
{
    exc3.DaysOfWeek.Add(dayType);
}

Console.WriteLine("Days of week for exception: " + exc3.Name);
foreach (var dayType in exc3.DaysOfWeek)
{
    Console.WriteLine("Day type: " + dayType);
}
```

### См. также

* enum [DayType](../../daytype/)
* class [DayTypeCollection](../)
* namespace [Aspose.Tasks](../../daytypecollection/)
* assembly [Aspose.Tasks](../../../)


