---
title: "Класс RecurringInterval"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Visualization.RecurringInterval. Представляет повторяющиеся интервалы, используемые в линиях прогресса представления диаграммы Ганта."
type: docs
weight: 3310
url: /ru/net/aspose.tasks.visualization/recurringinterval/
---
## RecurringInterval class

Представляет повторяющиеся интервалы, используемые в линиях прогресса представления диаграммы Ганта.

```csharp
public class RecurringInterval
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [RecurringInterval](recurringinterval/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [DailyDayNumber](../../aspose.tasks.visualization/recurringinterval/dailydaynumber/) { get; set; } | Получает или задает номер дня. |
| [DailyWorkday](../../aspose.tasks.visualization/recurringinterval/dailyworkday/) { get; set; } | Получает или задает значение, указывающее, является ли день рабочим для ежедневных линий прогресса. |
| [Interval](../../aspose.tasks.visualization/recurringinterval/interval/) { get; set; } | Получает или задает повторяющийся интервал. Может быть любым значением типа [`Interval`](./interval/). |
| [MonthlyDay](../../aspose.tasks.visualization/recurringinterval/monthlyday/) { get; set; } | Получает или задает значение, указывающее, показывать ли ежемесячные линии прогресса по дням. |
| [MonthlyDayDayNumber](../../aspose.tasks.visualization/recurringinterval/monthlydaydaynumber/) { get; set; } | Получает или задает номер дня ежемесячных линий прогресса. |
| [MonthlyDayMonthNumber](../../aspose.tasks.visualization/recurringinterval/monthlydaymonthnumber/) { get; set; } | Получает или задает номер месяца ежемесячных линий прогресса. |
| [MonthlyFirstLast](../../aspose.tasks.visualization/recurringinterval/monthlyfirstlast/) { get; set; } | Получает или задает значение, указывающее, показывать ли линии прогресса по первому или последнему предопределенному дню. |
| [MonthlyFirstLastDay](../../aspose.tasks.visualization/recurringinterval/monthlyfirstlastday/) { get; set; } | Получает или задает тип первого или последнего дня ежемесячных линий прогресса. |
| [MonthlyFirstLastMonthNumber](../../aspose.tasks.visualization/recurringinterval/monthlyfirstlastmonthnumber/) { get; set; } | Получает или задает номер месяца линий прогресса, которые отображаются по первому или последнему предопределенному дню. |
| [WeeklyDays](../../aspose.tasks.visualization/recurringinterval/weeklydays/) { get; } | Получает список дней для еженедельных линий прогресса. |
| [WeeklyWeekNumber](../../aspose.tasks.visualization/recurringinterval/weeklyweeknumber/) { get; set; } | Получает или задает номер недели для еженедельных линий прогресса. |

## Примеры

Показывает, как работать с повторяющимся интервалом линий прогресса.

```csharp
var project = new Project(DataDir + "Project2007.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[1];

// Позволяет читать линию прогресса
var interval = view.ProgressLines.RecurringInterval;

Console.WriteLine("Interval: " + interval.Interval);
Console.WriteLine("Weekly Week Number: " + interval.WeeklyWeekNumber);
foreach (var day in interval.WeeklyDays)
{
    Console.WriteLine("Week day: " + day);
}

// Позволяет переопределить повторяющийся интервал
var newInterval = new RecurringInterval();

// Устанавливает значение, указывающее, показывать ли месячные линии прогресса по дню.
interval.MonthlyDay = true;
// Устанавливает номер дня для месячных линий прогресса.
interval.MonthlyDayDayNumber = 1;
// Устанавливает номер месяца для месячных линий прогресса.
interval.MonthlyDayMonthNumber = 1;
// Устанавливает значение, указывающее, показывать ли линии прогресса по первому или последнему предопределённому дню.
interval.MonthlyFirstLast = true;
// Устанавливает тип первого или последнего дня для месячных линий прогресса.
interval.MonthlyFirstLastDay = RecurringInterval.DayType.Day;
// Устанавливает номер месяца для линий прогресса, которые отображаются по первому или последнему предопределённому дню.
interval.MonthlyFirstLastMonthNumber = 1;

view.ProgressLines.RecurringInterval = newInterval;

project.Save(OutDir + "WorkWithRecurringInterval_out.pdf", SaveFileFormat.Pdf);
```

### См. также

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


