---
title: "WorkingTime.WorkingTime"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "WorkingTime конструктор. Инициализирует новый экземпляр класса WorkingTime с интервалом, заданным указанными временем начала и окончания"
type: docs
weight: 10
url: /ru/net/aspose.tasks/workingtime/workingtime/
---
## WorkingTime(DateTime, DateTime) {#constructor_1}

Инициализирует новый экземпляр класса [`WorkingTime`](../) с интервалом, заданным указанными временем начала и окончания.

```csharp
public WorkingTime(DateTime fromTime, DateTime toTime)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fromTime | DateTime | время начала интервала |
| toTime | DateTime | время окончания интервала |

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

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)

---

## WorkingTime(TimeSpan, TimeSpan) {#constructor_2}

Инициализирует новый экземпляр класса [`WorkingTime`](../) с элементом интервала, заданным указанными временем начала и окончания.

```csharp
public WorkingTime(TimeSpan fromTime, TimeSpan toTime)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fromTime | TimeSpan | Время начала интервала, представленное структурой TimeSpan. |
| toTime | TimeSpan | Время окончания интервала, представленное структурой TimeSpan. |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | Когда toTime меньше или равен аргументу toTime или когда интервал между fromTime и toTime больше 24 часов. |

## Примеры

Перегрузка конструктора WorkingTime может использоваться для инициализации начала и конца интервала с помощью TimeSpans:

```csharp
[C#]
var wt = new WorkingTime(new TimeSpan(9, 0, 0), new TimeSpan(18, 0, 0));
```

### См. также

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)

---

## WorkingTime(int, int) {#constructor}

Инициализирует новый экземпляр класса [`WorkingTime`](../) с элементом интервала, заданным указанными временем начала и окончания.

```csharp
public WorkingTime(int fromHours, int toHours)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| fromHours | Int32 | Время начала интервала представлено целым числом часов (0‑24). |
| toHours | Int32 | Время окончания интервала представлено целым числом часов (0‑24). |

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentException | Когда toTime меньше или равен аргументу toTime или когда интервал между fromTime и toTime больше 24 часов. |

## Примеры

Перегрузка конструктора WorkingTime может использоваться для инициализации начала и конца интервала с помощью целых часов:

```csharp
[C#]
var wt = new WorkingTime(9, 13);
```

Показывает, как проверить равенство рабочего времени.

```csharp
var workingTime1 = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 17);

// Равенство календарей проверяется по датам начала и окончания рабочего времени.
Console.WriteLine("Working Time 1 (From): " + workingTime1.From);
Console.WriteLine("Working Time 1 (To): " + workingTime1.To);

Console.WriteLine("Working Time 2 (From): " + workingTime2.From);
Console.WriteLine("Working Time 2 (To): " + workingTime2.To);
Console.WriteLine("Are working times equal: " + workingTime1.Equals(workingTime2));
```

### См. также

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)


