---
title: "Класс WorkingTimeCollection"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.WorkingTimeCollection. Представляет коллекцию объектов WorkingTimeCollection."
type: docs
weight: 3670
url: /ru/net/aspose.tasks/workingtimecollection/
---
## WorkingTimeCollection class

Представляет коллекцию объектов `WorkingTimeCollection`.

```csharp
public class WorkingTimeCollection : IList<WorkingTime>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Count](../../aspose.tasks/workingtimecollection/count/) { get; } | Получает количество объектов, содержащихся в этом объекте `WorkingTimeCollection`. |
| [Item](../../aspose.tasks/workingtimecollection/item/) { get; set; } | Возвращает элемент по указанному индексу. |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.tasks/workingtimecollection/add/)(WorkingTime) | Добавляет новый экземпляр WorkingTime в эту коллекцию. |
| [Clear](../../aspose.tasks/workingtimecollection/clear/)() | Удаляет все элементы [`WorkingTime`](../workingtime/) из коллекции. |
| [Contains](../../aspose.tasks/workingtimecollection/contains/)(WorkingTime) | Проверяет, находится ли указанный элемент в List. Выполняет линейный поиск O(n). |
| [CopyTo](../../aspose.tasks/workingtimecollection/copyto/)(WorkingTime[], int) | копирует содержимое коллекции в Array, начиная с определённого индекса |
| [GetEnumerator](../../aspose.tasks/workingtimecollection/getenumerator/)() | Возвращает перечислитель для этой коллекции. |
| [Remove](../../aspose.tasks/workingtimecollection/remove/)(WorkingTime) | Удаляет экземпляр [`WorkingTime`](../workingtime/) из этой коллекции. |
| [ToList](../../aspose.tasks/workingtimecollection/tolist/)() | Преобразует объект WorkingTimeCollection в список объектов [`WorkingTime`](../workingtime/). |

## Примеры

Показывает, как работать с коллекцией рабочего времени.

```csharp
var project = new Project();
var calendar = project.Calendars.Add("Custom Calendar");

calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));

var saturdayWorkingTimes = new List<WorkingTime>
{
    new WorkingTime(8, 12),
    new WorkingTime(13, 15)
};
var saturday = new WeekDay(DayType.Saturday);
foreach (var time in saturdayWorkingTimes)
{
    saturday.WorkingTimes.Add(time);
}

// вывести рабочие часы субботы
Console.WriteLine("Saturday working period number: " + saturday.WorkingTimes.Count);
foreach (var time in saturday.WorkingTimes)
{
    Console.WriteLine("From Time: " + time.From);
    Console.WriteLine("To Time: " + time.To);
}

Console.WriteLine();

var sundayWorkingTimes = new List<WorkingTime>
{
    new WorkingTime(10, 15)
};
var sunday = new WeekDay(DayType.Sunday, sundayWorkingTimes);

// вывести рабочие часы воскресенья
List<WorkingTime> workingTimes = sunday.WorkingTimes.ToList();
Console.WriteLine("Sunday working period number: " + workingTimes.Count);
for (var index = 0; index < workingTimes.Count; index++)
{
    var time = workingTimes[index];
    Console.WriteLine("From Time: " + time.From);
    Console.WriteLine("To Time: " + time.To);
}

Console.WriteLine();

calendar.WeekDays.Add(saturday);
calendar.WeekDays.Add(sunday);

foreach (var day in calendar.WeekDays)
{
    Console.WriteLine(day.DayType + ": ");

    // Вы можете дальше проходить по рабочим часам и отображать их.
    foreach (var workingTime in day.WorkingTimes)
    {
        Console.WriteLine(workingTime.From);
        Console.WriteLine(workingTime.To);
    }

    Console.WriteLine();
}
```

### См. также

* class [WorkingTime](../workingtime/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


