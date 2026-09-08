---
title: "WeekDay.ToDate"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство WeekDay. Получает или задает конец периода исключения"
type: docs
weight: 60
url: /ru/net/aspose.tasks/weekday/todate/
---
## WeekDay.ToDate property

Получает или задает конец исключительного времени.

```csharp
public DateTime ToDate { get; set; }
```

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

* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)


