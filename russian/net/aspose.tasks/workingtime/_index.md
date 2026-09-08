---
title: "Класс WorkingTime"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.WorkingTime. Представляет рабочее время в будний день."
type: docs
weight: 3660
url: /ru/net/aspose.tasks/workingtime/
---
## WorkingTime class

Представляет рабочее время в течение дня недели.

```csharp
public class WorkingTime
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [WorkingTime](workingtime/#constructor_1)(DateTime, DateTime) | Инициализирует новый экземпляр класса `WorkingTime` с интервалом, заданным указанными временем начала и окончания. |
| [WorkingTime](workingtime/#constructor)(int, int) | Инициализирует новый экземпляр класса `WorkingTime` с элементом интервала, заданным указанными временем начала и окончания. |
| [WorkingTime](workingtime/#constructor_2)(TimeSpan, TimeSpan) | Инициализирует новый экземпляр класса `WorkingTime` с элементом интервала, заданным указанными временем начала и окончания. |

## Свойства

| Имя | Описание |
| --- | --- |
| [From](../../aspose.tasks/workingtime/from/) { get; } | Получает начало рабочего времени. |
| [To](../../aspose.tasks/workingtime/to/) { get; } | Получает конец рабочего времени. |

## Методы

| Имя | Описание |
| --- | --- |
| override [Equals](../../aspose.tasks/workingtime/equals/)(object) | Проверяет, что объекты равны. |
| override [GetHashCode](../../aspose.tasks/workingtime/gethashcode/)() | Возвращает значение хеш‑кода для экземпляра класса `WorkingTime`. |

## Примеры

Показывает, как работать с информацией о рабочем времени.

```csharp
public void WorkWithWorkingTime()
{
    var project = new Project();
    var calendar = CreateCalendar(project);
    project.Set(Prj.Calendar, calendar);

    Console.WriteLine("Work Week Number: " + calendar.WeekDays.Count);

    // Эти данные относятся к кнопке "Details." — здесь можно задать специальные рабочие часы для определённого дня недели или даже сделать его нерабочим.
    List<WeekDay> weekDays = calendar.WeekDays.ToList();
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
}

public static Calendar CreateCalendar(Project project)
{
    var calendar = project.Calendars.Add("MyCalendar", project.Calendars.GetByName("Standard"));
    var workingTimes = new List<WorkingTime>
                           {
                               new WorkingTime(new DateTime(1, 1, 1, 9, 0, 0), new DateTime(1, 1, 1, 12, 0, 0)),
                               new WorkingTime(new DateTime(1, 1, 1, 13, 0, 0), new DateTime(1, 1, 1, 18, 0, 0))
                           };

    calendar.WeekDays.Add(new WeekDay(DayType.Monday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Tuesday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Wednesday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Thursday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Friday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
    calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

    return calendar;
}
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


