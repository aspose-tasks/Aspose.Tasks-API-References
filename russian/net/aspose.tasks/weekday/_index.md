---
title: "Класс WeekDay"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.WeekDay. Представляет день недели, который либо определяет обычные дни недели, либо исключительные дни в календаре."
type: docs
weight: 3540
url: /ru/net/aspose.tasks/weekday/
---
## WeekDay class

Представляет день недели, который определяет либо обычные дни недели, либо исключительные дни в календаре.

```csharp
public class WeekDay
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [WeekDay](weekday/#constructor)() | Инициализирует новый экземпляр класса `WeekDay`. |
| [WeekDay](weekday/#constructor_1)(DayType) | Инициализирует новый экземпляр класса `WeekDay` с указанным типом дня. |
| [WeekDay](weekday/#constructor_3)(DayType, IEnumerable&lt;WorkingTime&gt;) | Инициализирует новый экземпляр класса `WeekDay` с указанным типом дня и списком рабочих периодов времени. |
| [WeekDay](weekday/#constructor_2)(DayType, params WorkingTime[]) | Инициализирует новый экземпляр класса `WeekDay` с указанным типом дня и рабочими периодами времени. |

## Свойства

| Имя | Описание |
| --- | --- |
| [DayType](../../aspose.tasks/weekday/daytype/) { get; } | Получает тип дня. |
| [DayWorking](../../aspose.tasks/weekday/dayworking/) { get; set; } | Получает или задает значение, указывающее, является ли указанная дата или тип дня рабочим. |
| [FromDate](../../aspose.tasks/weekday/fromdate/) { get; set; } | Получает или задает начало исключительного времени. |
| [ToDate](../../aspose.tasks/weekday/todate/) { get; set; } | Получает или задает конец исключительного времени. |
| [WorkingTimes](../../aspose.tasks/weekday/workingtimes/) { get; } | Получает WorkingTimeCollection для данного экземпляра WeekDay. Коллекция рабочих времён, определяющая время работы в этот день недели. |

## Методы

| Имя | Описание |
| --- | --- |
| static [CreateDefaultWorkingDay](../../aspose.tasks/weekday/createdefaultworkingday/)(DayType) | Создаёт рабочий день по умолчанию. |
| [Clone](../../aspose.tasks/weekday/clone/)() | Возвращает глубокую копию дня недели. |
| override [Equals](../../aspose.tasks/weekday/equals/)(object) | Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту. |
| override [GetHashCode](../../aspose.tasks/weekday/gethashcode/)() | Возвращает значение хеш‑кода для экземпляра класса `WeekDay`. |
| [GetWorkingTime](../../aspose.tasks/weekday/getworkingtime/)() | Возвращает рабочее время для дня недели. |
| static [CastToDayType](../../aspose.tasks/weekday/casttodaytype/)(DayOfWeek) | Преобразует DayOfWeek из .Net в [`DayType`](./daytype/). |
| static [SetDefaultWorkingTime](../../aspose.tasks/weekday/setdefaultworkingtime/)(WeekDay) | Устанавливает периоды времени по умолчанию для указанного дня недели. |

## Примеры

Показывает, как создать новый календарь, определяя дни недели.

```csharp
var project = new Project();

// Определить календарь
var calendar = project.Calendars.Add("Calendar1");

// Добавить рабочие дни с понедельника по четверг со стандартными часами
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(new WeekDay(DayType.Tuesday, new WorkingTime(9, 11), new WorkingTime(12, 18)));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));

var exceptionDay = WeekDay.CreateDefaultWorkingDay(DayType.Exception);
exceptionDay.FromDate = new DateTime(2020, 4, 27, 0, 0, 0);
exceptionDay.ToDate = new DateTime(2020, 4, 30, 0, 0, 0);
exceptionDay.DayWorking = false;
calendar.WeekDays.Add(exceptionDay);

// проверьте даты начала и окончания исключительного дня
Console.WriteLine("The from date is: " + exceptionDay.FromDate);
Console.WriteLine("The to date is: " + exceptionDay.ToDate);
Console.WriteLine();

calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// Установить пятницу как короткий рабочий день

// Устанавливает рабочее время. 
var workingTimes = new List<WorkingTime> { new WorkingTime(9, 12), new WorkingTime(13, 16) };

// существует способ преобразовать <see cref=\"DayOfWeek\" /> в <see cref=\"Aspose.Tasks.DayType\" />.
var dayType = WeekDay.CastToDayType(DayOfWeek.Friday);

var weekDay = new WeekDay(dayType, workingTimes);
weekDay.DayWorking = true;
Console.WriteLine("The day type is: " + weekDay.DayType);
Console.WriteLine("The from date is: " + weekDay.FromDate);
Console.WriteLine("The to date is: " + weekDay.ToDate);

calendar.WeekDays.Add(weekDay);

// выведем все рабочие времена
foreach (var day in calendar.WeekDays)
{
    Console.WriteLine("Day Type: " + day.DayType); 
    Console.WriteLine("Is working day: " + day.DayWorking); 
    Console.WriteLine("Working Time (Hours): " + day.GetWorkingTime().TotalHours);
    Console.WriteLine();
}
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


