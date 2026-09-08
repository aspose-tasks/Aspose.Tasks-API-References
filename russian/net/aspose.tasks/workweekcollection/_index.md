---
title: "Класс WorkWeekCollection"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.WorkWeekCollection. Представляет коллекцию объектов WorkWeek."
type: docs
weight: 3650
url: /ru/net/aspose.tasks/workweekcollection/
---
## WorkWeekCollection class

Представляет коллекцию объектов [`WorkWeek`](../workweek/).

```csharp
public class WorkWeekCollection : IList<WorkWeek>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Count](../../aspose.tasks/workweekcollection/count/) { get; } | Получает количество объектов, содержащихся в этом объекте `WorkWeekCollection`. |
| [Item](../../aspose.tasks/workweekcollection/item/) { get; set; } | Возвращает элемент по указанному индексу. |
| [ParentCalendar](../../aspose.tasks/workweekcollection/parentcalendar/) { get; } | Получает родительский календарь. |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.tasks/workweekcollection/add/)(WorkWeek) | Добавляет экземпляр WorkWeek в этот объект коллекции. |
| [GetEnumerator](../../aspose.tasks/workweekcollection/getenumerator/)() | Возвращает перечислитель для этой коллекции. |
| [ToList](../../aspose.tasks/workweekcollection/tolist/)() | Преобразует объект WorkWeekCollection в список объектов [`WorkWeek`](../workweek/). |

## Примеры

Показывает, как создать пользовательскую рабочую неделю для календаря.

```csharp
var project = new Project();
var calendar = project.Calendars.Add("Standard");
Calendar.MakeStandardCalendar(calendar);

var item = new WorkWeek();
item.Name = "My Work Week";
item.FromDate = new DateTime(2020, 4, 13, 8, 0, 0);
item.ToDate = new DateTime(2020, 4, 17, 17, 0, 0);
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));
item.WeekDays.Add(new WeekDay(DayType.Saturday));
item.WeekDays.Add(new WeekDay(DayType.Sunday));
calendar.WorkWeeks.Add(item);

Console.WriteLine("Work Weeks Count: " + calendar.WorkWeeks.Count);
foreach (var workWeek in calendar.WorkWeeks)
{
    // Отображает имя рабочей недели, имя родительского календаря, даты начала и окончания
    Console.WriteLine("Name: " + workWeek.Name);
    Console.WriteLine("Parent calendar name: " + calendar.Name);
    Console.WriteLine("From Date: " + workWeek.FromDate);
    Console.WriteLine("To Date: " + workWeek.ToDate);
    Console.WriteLine();

    // Эти данные относятся к кнопке "Details." — здесь можно задать специальные рабочие часы для определённого дня недели или даже сделать его нерабочим.
    List<WeekDay> weekDays = workWeek.WeekDays.ToList();
    foreach (var day in weekDays)
    {
        Console.WriteLine(day.DayType.ToString());

        // Вы можете дальше проходить по рабочим часам и отображать их.
        foreach (var workingTime in day.WorkingTimes)
        {
            Console.WriteLine(workingTime.From);
            Console.WriteLine(workingTime.To);
        }
    }

    Console.WriteLine();
}
```

### См. также

* class [WorkWeek](../workweek/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


