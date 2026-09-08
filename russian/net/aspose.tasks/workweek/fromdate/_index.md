---
title: "WorkWeek.FromDate"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство WorkWeek. Получает или задает дату и время начала рабочей недели"
type: docs
weight: 20
url: /ru/net/aspose.tasks/workweek/fromdate/
---
## WorkWeek.FromDate property

Получает или задает начальное DateTime рабочей недели

```csharp
public DateTime FromDate { get; set; }
```

## Примеры

Показывает, как прочитать информацию о рабочей неделе из проекта.

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

Console.WriteLine("Work Week Number: " + calendar.WeekDays.Count);
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

* class [WorkWeek](../)
* namespace [Aspose.Tasks](../../workweek/)
* assembly [Aspose.Tasks](../../../)


