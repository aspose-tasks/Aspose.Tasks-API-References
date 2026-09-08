---
title: "Класс DayTypeCollection"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.DayTypeCollection. Представляет коллекцию объектов DayType"
type: docs
weight: 460
url: /ru/net/aspose.tasks/daytypecollection/
---
## DayTypeCollection class

Представляет коллекцию объектов [`DayType`](../daytype/).

```csharp
public class DayTypeCollection : IList<DayType>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Count](../../aspose.tasks/daytypecollection/count/) { get; } | Получает количество элементов, содержащихся в этой коллекции. |
| [IsReadOnly](../../aspose.tasks/daytypecollection/isreadonly/) { get; } | Возвращает значение, указывающее, является ли эта коллекция только для чтения; иначе — false. |
| [Item](../../aspose.tasks/daytypecollection/item/) { get; set; } | Возвращает или задает элемент по указанному индексу. |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.tasks/daytypecollection/add/)(DayType) | Добавляет указанный элемент в эту коллекцию. |
| [Clear](../../aspose.tasks/daytypecollection/clear/)() | Удаляет все элементы из этой коллекции. |
| [Contains](../../aspose.tasks/daytypecollection/contains/)(DayType) | Возвращает true, если указанный элемент найден в этой коллекции; в противном случае — false. |
| [CopyTo](../../aspose.tasks/daytypecollection/copyto/)(DayType[], int) | Копирует элементы этой коллекции в указанный массив, начиная с указанного индекса массива. |
| [GetEnumerator](../../aspose.tasks/daytypecollection/getenumerator/)() | Возвращает перечислитель для этой коллекции. |
| [IndexOf](../../aspose.tasks/daytypecollection/indexof/)(DayType) | Определяет индекс указанного элемента в этой коллекции. |
| [Insert](../../aspose.tasks/daytypecollection/insert/)(int, DayType) | Вставляет указанный элемент в указанный индекс. |
| [Remove](../../aspose.tasks/daytypecollection/remove/)(DayType) | Удаляет первое вхождение конкретного объекта из этой коллекции. |
| [RemoveAt](../../aspose.tasks/daytypecollection/removeat/)(int) | Удаляет элемент по указанному индексу. |

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

* enum [DayType](../daytype/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


