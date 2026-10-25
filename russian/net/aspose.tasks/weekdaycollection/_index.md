---
title: "Класс WeekDayCollection"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.WeekDayCollection. Представляет коллекцию объектов WeekDay"
type: docs
weight: 3550
url: /ru/net/aspose.tasks/weekdaycollection/
---
## WeekDayCollection class

Представляет коллекцию объектов [`WeekDay`](../weekday/).

```csharp
public class WeekDayCollection : IList<WeekDay>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Count](../../aspose.tasks/weekdaycollection/count/) { get; } | Получает количество объектов, содержащихся в этом объекте `WeekDayCollection`. |
| [Item](../../aspose.tasks/weekdaycollection/item/) { get; set; } | Получает или задает значение элемента по указанному индексу. |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.tasks/weekdaycollection/add/)(WeekDay) | Добавляет экземпляр [`WeekDay`](../weekday/) в этот объект. |
| [Clear](../../aspose.tasks/weekdaycollection/clear/)() | Очищает объект WeekDayCollection. |
| [Contains](../../aspose.tasks/weekdaycollection/contains/)(WeekDay) | Проверяет, содержит ли коллекция указанный [`WeekDay`](../weekday/). |
| [CopyTo](../../aspose.tasks/weekdaycollection/copyto/)(WeekDay[], int) | Копирует содержимое коллекции в массив по указанному индексу. |
| [GetEnumerator](../../aspose.tasks/weekdaycollection/getenumerator/)() | Возвращает перечислитель для этой коллекции. |
| [IndexOf](../../aspose.tasks/weekdaycollection/indexof/)(WeekDay) | Возвращает индекс указанного [`WeekDay`](../weekday/). |
| [Insert](../../aspose.tasks/weekdaycollection/insert/)(int, WeekDay) | Вставляет [`WeekDay`](../weekday/) по указанному индексу. |
| [Remove](../../aspose.tasks/weekdaycollection/remove/)(WeekDay) | Удаляет указанный [`WeekDay`](../weekday/), если он существует. |
| [RemoveAt](../../aspose.tasks/weekdaycollection/removeat/)(int) | Удаляет элемент по указанному индексу. |
| [ToList](../../aspose.tasks/weekdaycollection/tolist/)() | Преобразует объект WeekDayCollection в список объектов [`WeekDay`](../weekday/). |

## Примеры

Показывает, как работать с коллекциями дней недели.

```csharp
var project = new Project();
var calendar = project.Calendars.GetByName("Standard");

// очистить дни недели
calendar.WeekDays.Clear();

calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));
var saturday = WeekDay.CreateDefaultWorkingDay(DayType.Saturday);
var sunday = WeekDay.CreateDefaultWorkingDay(DayType.Sunday);

calendar.WeekDays.Add(saturday);
calendar.WeekDays.Add(sunday);

var fridayWorkingTimes = new List<WorkingTime> { new WorkingTime(new DateTime(2020, 4, 13, 8, 0, 0), new DateTime(2020, 4, 13, 12, 0, 0)) };

var friday = new WeekDay(DayType.Friday, fridayWorkingTimes);
if (calendar.WeekDays.Contains(friday))
{
    calendar.WeekDays.Insert(4, friday);
}

Console.WriteLine("Calendar: " + calendar.Name);
Console.WriteLine("Week days count: " + calendar.WeekDays.Count);
foreach (var day in calendar.WeekDays)
{
    Console.WriteLine(day.DayType);
    foreach (var workingTime in day.WorkingTimes)
    {
        Console.WriteLine("From: " + workingTime.From);
        Console.WriteLine("To: " + workingTime.To);
        Console.WriteLine();
    }
}

// удалить субботний день недели
calendar.WeekDays.RemoveAt(5);

// удалить воскресный день недели
if (calendar.WeekDays.IndexOf(saturday) > 0)
{
    calendar.WeekDays.Remove(sunday);
}

Console.WriteLine("Working times after weekend was removed: ");
List<WeekDay> weekDays = calendar.WeekDays.ToList();
foreach (var day in weekDays)
{
    Console.WriteLine(day.DayType);
    foreach (var workingTime in day.WorkingTimes)
    {
        Console.WriteLine("From: " + workingTime.From);
        Console.WriteLine("To: " + workingTime.To);
        Console.WriteLine();
    }
}

var hour24Calendar = project.Calendars.Add("24 Hours");
Calendar.Make24HourCalendar(hour24Calendar);

// скопировать дни недели
var weekDaysArray = new WeekDay[calendar.WeekDays.Count];
calendar.WeekDays.CopyTo(weekDaysArray, 0);

foreach (var weekDay in weekDaysArray)
{
    hour24Calendar.WeekDays.Add(weekDay);
}
```

### См. также

* class [WeekDay](../weekday/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


